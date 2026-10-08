# EduTrack Data Audit

## 1. Enrollments in 'Intro to Python'

Result: 5 enrollments

| Student | Email | Completion |
|---|---|---:|
| Emily Watson | emily.watson@student.edutrack.com | 85% |
| Klaus Weber | klaus.weber@student.edutrack.com | 92% |
| Marco Rossi | marco.rossi@student.edutrack.com | 88% |
| James Miller | james.miller@test.com | 30% |
| Priya Sharma | priya.sharma@student.edutrack.com | 55% |

## 2. Potential dropouts

Result: 4 enrollments have a completion percentage below 10.

| ID | Student | Email | Course | Category | Enrollment date | Completion | Passed | Fee paid | Instructor |
|---:|---|---|---|---|---|---:|---|---:|---|
| 5 | Lucia Fernandes | lucia.fernandes@student.edutrack.com | Web Design Basics | Design | 2024-06-20 | 5% | false | $39.99 | Carlos Vega |
| 6 | Lucia Fernandes | lucia.fernandes@student.edutrack.com | Digital Marketing 101 | Marketing | 2024-07-01 | 3% | false | $29.99 | Lucia Prades |
| 10 | Yuki Nakamura | yuki.nakamura@student.edutrack.com | UI/UX Fundamentals | Design | 2024-10-11 | 0% | false | $44.99 | NULL |
| 11 | Pierre Dubois | pierre.dubois@student.edutrack.com | UI/UX Fundamentals | Design | 2024-11-05 | 0% | false | $44.99 | NULL |

## 3. Enrollments with no instructor

Result: 2 enrollments have a NULL instructor.

| ID | Student | Email | Course | Category | Enrollment date | Completion | Passed | Fee paid | Instructor |
|---:|---|---|---|---|---|---:|---|---:|---|
| 10 | Yuki Nakamura | yuki.nakamura@student.edutrack.com | UI/UX Fundamentals | Design | 2024-10-11 | 0% | false | $44.99 | NULL |
| 11 | Pierre Dubois | pierre.dubois@student.edutrack.com | UI/UX Fundamentals | Design | 2024-11-05 | 0% | false | $44.99 | NULL |

## 4. Five highest-completion students who have not passed

Result:

| Student | Course | Completion |
|---|---|---:|
| Emily Watson | Web Design Basics | 60% |
| Priya Sharma | Intro to Python | 55% |
| Yuki Nakamura | Data Analysis with SQL | 45% |
| Emily Watson | Advanced Python | 40% |
| James Miller | Intro to Python | 30% |

## 5. Enrollments created in the last year

Result: 0 enrollments.

The query uses the current database date minus one year. The newest starter-data enrollment is dated 2025-03-05, so none fall within the year ending 2026-10-06.

## 6. Missing enrollment inserted

Result: 1 enrollment added.

| ID | Student | Email | Course | Category | Enrollment date | Completion | Passed | Fee paid | Instructor |
|---:|---|---|---|---|---|---:|---|---:|---|
| 18 | Lucia Fernandes | lucia.fernandes@student.edutrack.com | Advanced Python | Programming | 2025-04-01 | 0% | false | $69.99 | Carlos Vega |

## 7. Missing instructors corrected

Result: 2 enrollments updated. Their instructor is now `Pending assignment`.

| ID | Student | Course | New instructor |
|---:|---|---|---|
| 10 | Yuki Nakamura | UI/UX Fundamentals | Pending assignment |
| 11 | Pierre Dubois | UI/UX Fundamentals | Pending assignment |

## 8. Test-account enrollments deleted

Result: 2 enrollments deleted. No non-test enrollment was removed.

| ID | Student | Email | Course |
|---:|---|---|---|
| 13 | James Miller | james.miller@test.com | Intro to Python |
| 14 | Alex Chen | alex.chen@test.com | Web Design Basics |

## 9. Enrollments by category

Result:

- Programming: 7
- Design: 4
- Data: 3
- Marketing: 2

## 10. Average completion by course

Result, ordered from lowest to highest:

| Course | Average completion |
|---|---:|
| UI/UX Fundamentals | 0.00% |
| Web Design Basics | 32.50% |
| Digital Marketing 101 | 36.50% |
| Advanced Python | 45.00% |
| Data Analysis with SQL | 47.67% |
| Intro to Python | 80.00% |

## 11. Courses with more than 3 enrollments

Result:

- Intro to Python: 4

## 12. Revenue by category

Result, ordered from highest to lowest:

| Category | Total revenue |
|---|---:|
| Programming | $409.93 |
| Data | $179.97 |
| Design | $169.96 |
| Marketing | $59.98 |
