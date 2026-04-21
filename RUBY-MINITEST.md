**Testing**
- Use `Minitest::Mock` for mocking external dependencies (classes, services)
  - Mock instances with `mock = Minitest::Mock.new; mock.expect(:method, return_value, [args])`
  - Use `assert_mock(mock)` to verify expectations
  - Use `Constant.stub :method, mock do ... end` to override a single method for the duration of the block
