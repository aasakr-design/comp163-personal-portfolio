# comp163-personal-portfolio
Personal portfolio project for COMP 163
# === DATA STORAGE ===

# Strings
full_name = "Abdelrahman Sakr"
student_email = "aasakr@aggies.ncat.edu"
hometown = "Chapel Hill, NC"
graduation_semester = "Fall 2029"
major = "Computer Science"

# Lists
current_courses = ["COMP 163", "COMP 390", "ENGL 100", "GEEN 111", "HIST 106"]
credit_hours = [3, 3, 3, 3, 3]
gpa_history = []  # None yet
completed_courses = []  # None yet

# Tuples
emergency_contact = ("Mom", "Hannah Smith", "929-208-9422")
home_address = ("Your Street Address", "Chapel Hill, NC", "27514")
instagram_info = ("Instagram", "@3bdou_sakr", 673)

# Sets
current_skills = {"Python", "Problem-Solving"}
skills_to_learn = {"Strengthen coding fundamentals", "Improve study habits"}
career_interests = {"Software Engineer", "Cybersecurity Analyst"}
hobbies = {"Soccer", "Photography"}
entertainment_backlog = set()  # optional

# Dictionaries
course_professors = {
    "COMP 163": "Prof. Rhodes",
    "COMP 390": "Dr. [Instructor]",
    "ENGL 100": "Dr. [Instructor]",
    "GEEN 111": "Dr. [Instructor]",
    "HIST 106": "Dr. [Instructor]"
}

course_rooms = {
    "COMP 163": "M-Eric 300",
    "COMP 390": "Marteena 201",
    "ENGL 100": "Crosby 121",
    "GEEN 111": "Room 101",
    "HIST 106": "Crosby 210"
}

monthly_budget = {"Food": 250, "Entertainment": 150, "Books": 100, "Transportation": 100}
study_hours = {"Programming": 8}  # weekly study hours
contact_directory = {"Mom": "929-208-9422", "Roommate": "336-555-7821", "Academic Advisor": "336-334-5000"}

# === CALCULATIONS ===
total_current_credits = sum(credit_hours)
cumulative_gpa = sum(gpa_history)/len(gpa_history) if gpa_history else 0
completed_courses_count = len(completed_courses)
total_weekly_study_hours = sum(study_hours.values())
academic_load = total_current_credits + total_weekly_study_hours
monthly_budget_total = sum(monthly_budget.values())
daily_food_budget = monthly_budget["Food"] / 30
annual_budget_projection = monthly_budget_total * 12
study_cost_per_hour = monthly_budget["Books"] / total_weekly_study_hours if total_weekly_study_hours else 0
total_followers = instagram_info[2]

# === OUTPUT ===
print("==================")
print("==============================================")
print("         PERSONAL ACADEMIC & LIFE PORTFOLIO")
print("==============================================")
print("==================")

print(f"Student: {full_name} | Email: {student_email}")
print(f"From: {hometown} | Graduating: {graduation_semester}")
print(f"Major: {major}")

print("=== ACADEMIC PROFILE ===")
print(f"Current Semester: {total_current_credits} credits across {len(current_courses)} courses")
print(f"Cumulative GPA: {cumulative_gpa:.2f}")
print(f"Weekly Study Time: {total_weekly_study_hours} hours")
print(f"Academic Investment: ${study_cost_per_hour:.1f} per study hour")

print("Current Courses:")
for i, course in enumerate(current_courses):
    print(f"{course} - {credit_hours[i]} credits - {course_professors[course]} - {course_rooms[course]}")

print("=== PERSONAL DEVELOPMENT ===")
print(f"Current Skills: {current_skills}")
print(f"Learning Goals: {skills_to_learn}")
print(f"Career Interests: {career_interests}")
print(f"Skills Currently Have: {len(current_skills)}")
print(f"Skills Want to Learn: {len(skills_to_learn)}")

print("=== FINANCIAL OVERVIEW ===")
print(f"Monthly Budget: ${monthly_budget_total}")
print(f"Food: ${monthly_budget['Food']} (${daily_food_budget:.1f}/day)")
print(f"Entertainment: ${monthly_budget['Entertainment']}")
print(f"Books: ${monthly_budget['Books']}")
print(f"Transportation: ${monthly_budget['Transportation']}")
print(f"Annual Projection: ${annual_budget_projection}")

print("=== CONNECTIONS & CONTACTS ===")
print(f"Emergency Contact: {emergency_contact[1]} ({emergency_contact[0]}) - {emergency_contact[2]}")
print(f"Home Address: {home_address[0]}, {home_address[1]} {home_address[2]}")
print(f"Social Media Presence: {total_followers} followers across 1 platform")
print(f"Key Contacts: {len(contact_directory)} people in directory")

print("=== LIFE STATISTICS ===")
print(f"Total Courses Completed: {completed_courses_count}")
print(f"Current Academic Load: {academic_load} weekly commitments")
print(f"Entertainment Backlog: {len(entertainment_backlog)} items")
print(f"Current Hobbies: {len(hobbies)} activities")

print("==================")
print("==============================================")

# === AI Assistance Note ===
# Some code formatting guidance was provided by AI (ChatGPT) per course policy




