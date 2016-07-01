# Form Requests

In Form Submission and validation use requests
```php
// Create Form Request

php artisan make:request SubmissionFormRequest


// Under method rules() define rules for form fields

 public function rules()
    {
        return [
            'field' => 'required|numeric'
        ];
    }
```
If form validation failed after your AJAX callback. Then Laravel may prompt '422 unprocessable entity laravel'
Solution for that : In ajax callback for error, use error response to display error.

