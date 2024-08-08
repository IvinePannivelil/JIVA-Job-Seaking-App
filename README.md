                                                                                  Jiva Job-Seeking App


Description: Jiva is a job-seeking application designed to connect job seekers with potential employers. It provides functionalities for users to view job listings, apply for jobs, and manage their applications. The application includes features such as user authentication, job browsing, and application management.
________________________________________
Key Components
1. HeadlineWidget
Purpose: Displays a section title with an optional action text and callback function.
Details:
•	Title: Main title displayed in the widget.
•	Action Text: Optional text that appears as an action button. If provided, it is displayed on the right side of the title.
•	Callback Function: Optional function that is triggered when the action text is tapped.
2. Job Class
Purpose: Represents a job listing with various attributes.
Attributes:
•	companyName: Name of the company offering the job.
•	companyImage: Path to the company's logo image.
•	jobTitle: Title of the job position.
•	location: Full location of the job.
•	locationShort: Abbreviated location.
•	salary: Salary range or amount for the job.
•	jobType: Type of job (e.g., Full Time, Part Time).
•	requirements: List of job requirements.
•	about: Description of the job and the company.
•	timeStamp: Time since the job was posted.
3. Login Screen
Purpose: Provides user authentication functionality.
Features:
•	Username and Password Fields: Input fields for user credentials.
•	Visibility Toggle: Button to show or hide the password.
•	Validation: Checks if the entered credentials match hardcoded values.
•	Navigation: Redirects users to either the home screen or login screen based on authentication.
4. SplashScreen
Purpose: Initial screen displayed when the application starts.
Features:
•	Logo Display: Shows the application's logo with a gradient background.
•	Text: Displays motivational text and a description of the app’s purpose.
•	Navigation: Determines the next screen based on stored user preferences (e.g., login or home screen).
5. RecentJobWidget
Purpose: Displays a list of recent job postings.
Features:
•	Job List: Shows a scrollable list of job postings with company logo, job title, location, and job type.
•	Navigation: Tapping on a job listing navigates to a detailed job view.
6. TipsWidget
Purpose: Displays rotating job application tips.
Features:
•	Rotating Tips: Shows a series of tips with automatic rotation every few seconds.
•	UI Elements: Includes circular indicators and background decorations for visual appeal.
7. ViewApplicationScreen
Purpose: Allows users to view details of their job application.
Features:
•	Application Data: Displays information such as name, date of birth, qualifications, and experience.
•	Data Loading: Retrieves application data from SharedPreferences.
________________________________________
Application Flow
1.	Splash Screen: On launch, the splash screen is displayed. It checks for stored user information to determine whether to show the login screen or the home screen.
2.	Login Screen: Users enter their credentials to access the application. Valid credentials lead to the home screen, while invalid ones prompt an error message.
3.	Home Screen: Displays recent job listings and tips for job seekers. Users can browse job postings and view detailed information about each job.
4.	View Application Screen: Allows users to view the details of their job applications stored locally.
________________________________________
Design and Themes
Colors: The application uses a primary color theme (AppColor.primaryColor) for visual consistency. Backgrounds and UI elements are designed to be appealing and user-friendly.
Themes: Custom themes are applied throughout the app to maintain a cohesive look and feel.
________________________________________
Navigation
•	AppRoute: Manages navigation between screens using named routes.
•	SharedPreferences: Used for storing and retrieving user-specific data, such as login information and application details.
________________________________________
Conclusion
Jiva is a feature-rich job-seeking application designed to enhance the job search experience. With its user-friendly interface, efficient navigation, and comprehensive functionality, it aims to provide a seamless experience for job seekers.

