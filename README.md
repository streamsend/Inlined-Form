# Inlined-Form
Download the example.html file from this repo and use as a starting point. 

## Configuration
Update the configuration block with information.

```
ss_thank_you_message = "Thank you for signing up.";
ss_event_name        = "StreamSend Signup Form";
ss_account_id        = 1234;
```
### ss_thank_you_message
The message that will show when the form is completed.

### ss_event_name 
The event name that shows up for automation purposes (if the account has option enabled)

### ss_account_id
The id number for the account


## Styles
Configure the styles

```
/* class for all fields with errors */
.field-error {background: red;}

/* class for error message */
.streamsend-error {background: red; }

/* id for the streamsend form */
#streamsend_form { }

/* id for the streamsend form success message */
#streamsend_form_success {color: green; }

/* id for the email address input */
#email_address { }

/* id for the submit button */
#streamsend-submit { }
```

## Update the form HTML
In some cases the HTML may need to be updated, for example, if you want to remove the Email label in front of the textfield. 

```
<form id="streamsend_form" name="streamsend_form" method="post">
    <div>
        <label>Email</label>
        <input placeholder="Email" type="1email" id="email_address" name="email_address" tabindex="1" autofocus />
        <button type="submit" name="submit" id="streamsend-submit" tabindex="10">Send</button>
        <div id="streamsend-error" class="streamsend-error"></div>
    </div>
</form>
<div id="streamsend_form_success"></div>
```

