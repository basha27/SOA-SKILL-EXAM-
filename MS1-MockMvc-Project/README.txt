MS1 - MockMvc Controller Testing

Import into Spring Tool Suite (STS):
1. Extract this ZIP file.
2. Open STS.
3. Select File > Import > Maven > Existing Maven Projects.
4. Browse to the extracted MS1-MockMvc-Project folder.
5. Select the pom.xml and click Finish.
6. Wait for Maven dependencies to download.

Run the test:
1. Open src/test/java/com/example/demo/MS1ControllerTest.java.
2. Right-click the file.
3. Select Run As > JUnit Test.
4. Confirm that the test passes.

Expected response:
HTTP 200 OK
MS 1.1 - Additon = 15

Requirements:
- JDK 17 or later
- Maven (STS can use its embedded Maven)
- Internet connection on first import to download dependencies

Note:
The controller has no service dependency, so no mocked dependency is required
for this particular test. @WebMvcTest loads the web layer and MockMvc
performs the simulated HTTP request without starting a real web server.
