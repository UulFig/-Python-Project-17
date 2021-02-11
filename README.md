# -Python-Project-17
#17 Average weight calculation using Loop


student_heights = input("Input a list of student heights ").split()
for n in range(0, len(student_heights)):
  student_heights[n] = int(student_heights[n])

total_heights = 0

for x in student_heights:
    total_heights += x
print(f"The total height is: {total_heights}")

total_students = 0

for students in student_heights:
    total_students += 1
print(f"The total students is: {total_students}")

avg = total_heights / total_students
print(f"The average height is: {round(avg,2)}\n")

higher_height = 0

for height in student_heights:
    if height > higher_height:
        higher_height = height
print(f"The higher height is {higher_height}")

lower_height = higher_height

for height in student_heights:
    if lower_height > height:
        lower_height = height
print(f"The lower height is {lower_height}")
