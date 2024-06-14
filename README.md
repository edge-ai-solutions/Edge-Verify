EdgeVerify Apps
Technology Used: - Firebase ML-Vision for Text Recognize.

Core Technology:
Edge AI OCR: A pre-trained deep learning model embedded directly on the tablet or phone camera performs real-time OCR. This eliminates the need for constant internet connection and ensures data privacy as text extraction and verification occur locally on the device.
Document Verification (Optional): For enhanced security, document verification can be integrated as a secondary layer. This feature compares extracted text data (e.g., ID numbers, names) against a secure database or online verification services (may require internet access).

Use Cases:

1. Event Check-in:

Benefits:
		Expedite event check-in processes by quickly scanning and verifying attendee IDs.
		Reduce wait times and improve overall event flow.
		Eliminate manual data entry errors and ensure accurate attendance records.

Implementation:
		Event staff use tablets or phones equipped with the app to scan attendees' ID documents (e.g., tickets, passports).
		The app utilizes Edge AI OCR to extract relevant information like names, ID numbers, and event codes.
		The extracted data is verified against a pre-loaded event guest list or connected to an online verification service (if internet available) for authentication.

2.Customer Onboarding:

Benefits:
		Streamline customer onboarding processes by quickly capturing and verifying identity documents.
		Improve customer experience by eliminating lengthy paperwork procedures.
		Reduce errors and ensure accurate customer data collection.

Implementation:
		Businesses can utilize the app for customer onboarding, scanning IDs such as driver's licenses or passports.
		Edge AI OCR extracts relevant customer information automatically.
		This data can be used for pre-filling customer applications or compared against a verification database for KYC (Know Your Customer) compliance.

3.Age Verification:

Benefits:
		Enhance age verification processes in age-restricted environments (e.g., bars, gambling establishments).
		Improve compliance with age verification regulations.
		Reduce the risk of serving underage individuals.

Implementation:
		Businesses can use the app to scan and verify government-issued IDs with birthdates.
		Edge AI OCR extracts the birthdate and compares it to a pre-set age threshold.
		Access is granted only to verified individuals of legal age.

3.High-Security Areas:

Benefits:
		Provides an additional layer of security for restricted areas.
		Verifies identity through a combination of OCR and document verification (optional).
		Maintains a detailed record of access attempts for audit purposes.

Implementation:
		This scenario utilizes both Edge AI OCR and document verification.
		Upon entry attempts, the system first performs OCR on relevant documents (e.g., employee ID badges).
		Extracted data is then compared against a secure database or online verification service for authentication (may require internet).
		Only authorized personnel with successful verification are granted access.


App Benefits:
			
			1.Offline Functionality: The app can operate entirely on the device, eliminating reliance on internet connectivity for core functionalities.

			2.Enhanced Security: Edge AI processing ensures data privacy by keeping text extraction and initial verification local (if applicable).
			
			3.Data Security: Sensitive information can be encrypted before any optional online verification for additional security.
			
			4.Improved Efficiency: Streamlines identity verification processes and reduces manual data entry tasks.
			
			5.Scalability: The platform can be easily scaled to accommodate different sized organizations and locations.

This AI-powered OCR platform offers a versatile and secure solution for identity verification across various scenarios. By leveraging Edge AI technology, it provides a reliable and efficient way to verify identities while maintaining data privacy and security.


Add it in your root build.gradle at the end of repositories:

dependencyResolutionManagement 
{
		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
		repositories 
		{
			mavenCentral()
			maven { url 'https://jitpack.io' }
		}

}
