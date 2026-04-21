Create a Student Registration Form using Angular.

The form must collect:
* Full Name
* Email
* Age
* Password
* Confirm Password
* Department
* Accept Terms

## Requirements

### 1) Use Reactive Forms
Create the form with `FormGroup` and `FormControl` or `FormBuilder`.
### 2) Use built-in validators
Apply these validations:
* **Full Name**

  * required
  * minimum length: 3

* **Email**

  * required
  * valid email format

* **Age**

  * required
  * minimum: 18

* **Password**

  * required
  * minimum length: 8

* **Department**

  * required

* **Accept Terms**

  * must be checked

### 3) Use one custom validator

Create a custom validator to check that:

* **Password** and **Confirm Password** must match

Show a clear error message when they do not match.

### 4) Use a service

Create a service called, for example, `student.service.ts`.

The service should:

* contain a method to submit form data
* use `HttpClient`
* send the form data to a fake API endpoint such as:

  * `https://jsonplaceholder.typicode.com/posts`

### 5) Use signals

Use Angular **signal** to manage at least:

* submission state, such as `isSubmitting`
* disable submit button while sending request
* success message or submitted result

### 6) Error display

Show validation messages only after the field is touched, or the form is submitted

### 7) Submission behavior

When the form is valid and submitted:

* call the service
* send data with `HttpClient`
* show returned result or success message
* reset the form after successful submission
