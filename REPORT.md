# Lab 3 Complete a Web API -- Project Report

## Description of Changes
- Added blocks to fun `POST is not safe and not idempotent`():
    - Setup for the method `save` to return first an employee with an ID and then the same employee with different ID
    - Verify to check that the method `save` was called exactly twice.

- Added blocks to fun `GET is safe and idempotent`():
    - Setup for the method `findById` to return employee `Mary` when called with argument "1" and empty when called with argument "2".
    - Verify to check that method `findById` with argument "1" was called exactly twice and that other methods weren't called.

- Added blocks to fun `PUT is idempotent but not safe`():
    - Setup for the method `findById` to return empty when called for the first time and data of an employee when called afterwards.
    - Setup for method `save` to return fakely saved info of a determined employee.
    - Verify to check that the method `findById` was called exactly twice with argument "1" and that the method `save` was called exactly twice.

- Added blocks to fun `DELETE is idempotent but not safe`():
    - Setup for method `findById` to return data about an employee when called for the first time with argument "1" and empty when called afterwards with the same argument.
    - Verify to check that the method `deleteById` was called exactly twice and other methods weren't called.

## Technical Decisions
No technical decisions were made during the development of this lab. Everything was on the script.

## Learning Outcomes
Use of setup and verify blocks to create quality tests to control the correct performance of the application.

## AI Disclosure
### AI Tools Used
No AI was used during the development of this lab.

### AI-Assisted Work
None

### Original Work
Every added change (following the script)