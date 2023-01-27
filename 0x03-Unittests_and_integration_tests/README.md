Unittests_and_integration_tests

file description

0. Familiarize yourself with the utils.access_nested_map function and understand its purpose. Play with it in the Python console to make sure you understand.
1. Implement TestAccessNestedMap.test_access_nested_map_exception. Use the assertRaises context manager to test that a KeyError is raised for the following inputs (use @parameterized.expand)
2. Define the TestGetJson(unittest.TestCase) class and implement the TestGetJson.test_get_json method to test that utils.get_json returns the expected result.
3. Implement the TestMemoize(unittest.TestCase) class with a test_memoize method.
4. In a new test_client.py file, declare the TestGithubOrgClient(unittest.TestCase) class and implement the test_org method.
5. memoize turns methods into properties. Read up on how to mock a property (see resource) and Implement the test_public_repos_url method to unit-test GithubOrgClient._public_repos_url
6.  Implement TestGithubOrgClient.test_public_repos to unit-test GithubOrgClient.public_repos
7.  Implement TestGithubOrgClient.test_has_license to unit-test GithubOrgClient.has_license
8.  We want to test the GithubOrgClient.public_repos method in an integration test. That means that we will only mock code that sends external requests
9.  Implement the test_public_repos method to test GithubOrgClient.public_repos.
