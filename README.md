 POE – Parts 1, 2 and 3
 
## Implemented areas
- Part 1: registration, username/password/cellphone validation, login.
- Part 2: message IDs, recipient and length validation, SHA-256 message hash, send/store/disregard actions, sent-message counter.
- Part 3: message arrays, longest sent message, search by ID, search by recipient, delete by hash, sent-message report, JSON export/read/display.

## JSON demonstration
Run the application and:
1. Send at least one message.
2. Select menu option 9 to write sent messages to `messages.json`.
3. Select menu option 10 to read the JSON file into a `Message[]` array and display it.

The JSON file is created in the application's working directory. The JSON helper supports the structure written by this application.

## Tests
- `test/QuickChatTest.java` contains JUnit 5 tests. Add JUnit 5 to the project's Test Libraries to execute it from NetBeans.
- `testng/QuickChatTestNG.java` contains TestNG automated tests to address the rubric's TestNG requirement. Add TestNG to NetBeans Test Libraries before running these tests. The TestNG source is kept separate from the Ant default test source folder to avoid compilation errors on machines without the TestNG library.

## Important notes
- Message data is held in arrays while the application is running. JSON export is an explicit operation; data is not automatically persistent unless exported.
- The program validates and processes messages locally. It does not send real SMS messages.
- Review the assignment's exact required message-hash formula and cellphone format with your lecturer's specification before submission.
- Do not claim tests pass until you have run them in your own NetBeans environment.
