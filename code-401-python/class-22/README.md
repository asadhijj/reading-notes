# Django CRUD and Forms

## Django Forms

    An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

**Form Attributes**

    action: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.
    method: The HTTP method used to send the data: post or get.

    The POST method should always be used if the data is going to result in a change to the server's database, because it can be made more resistant to cross-site forgery request attacks.
    The GET method should only be used for forms that don't change user data (for example, a search form). It is recommended for when you want to be able to bookmark or share the URL.

**Django Form Handling**

    Display the default form the first time it is requested by the user.
    Receive data from a submit request and bind it to the form.
    Clean and validate the data.
    If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.
    If all data is valid, perform required actions (such as save the data, send an email, return the result of a search, upload a file, and so on).
    Once all actions are complete, redirect the user to another page.

**How to declare a form?**

    Form data is stored in an application's forms.py file, inside the application directory. Create and open the file locallibrary/catalog/forms.py. To create a Form, we import the forms library, derive from the Form class, and declare the form's fields. A very basic form class for our library book renewal form is shown below ??? add this to your new file:

from django import forms class RenewBookForm(forms.Form): renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")
Common form fields

    BooleanField
    CharField
    ChoiceField
    TypedChoiceField
    DateField
    DateTimeField
    DecimalField
    DurationField

**Common form fields arguments:**

    required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.
    label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).
    label_suffix: By default, a colon is displayed after the label (e.g. Renewal date???:). This argument allows you to specify a different suffix containing other character(s).
    initial: The initial value for the field when the form is displayed.
    widget: The display widget to use.
    help_text (as seen in the example above): Additional text that can be displayed in forms to explain how to use the field.
    error_messages: A list of error messages for the field. You can override these with your own messages if needed.
    validators: A list of functions that will be called on the field when it is validated.
    localize: Enables the localization of form data input (see link for more information).
    disabled: The field is displayed but its value cannot be edited if this is True. The default is False.
