# How to Use

This goes over the sections of the code you will need to change in order to use the form. As well as instructions on how to change the subject dropdown.

## SITE KEYS

Make sure you change the SITE KEY on the `index.html` at this line:
`<div class="g-recaptcha" style="float: right;" data-sitekey="DATA-SITE-KEY"></div>`

Make sure you change the SECRET KEY on the `contact.php` file at this line:
`$secret = "SECRET-KEY-HERE"; //your recaptcha SECRET KEY`

<<<<<<< HEAD
### 📧 EMAIL FOR CONTACT FORM

You will change the email in this function to the email you would like responses from the form to be sent to. This is located in the contact.php file. The email currently in place is `szy17604@boofx.com`

    if ($success == false)
    //This user was not verified by recaptcha
    echo "Recaptcha Verification Failed";
    } else if ($success == true) {
    //This user is verified by recaptcha
    if (mail("szy17604@boofx.com", $subject, $Body, $headers)){
    //send successful
    echo "Recaptcha Success, Mail Sent Successfully";
    }else{
    //send failure
    echo "Mailing Failed";
    }
    }

### 🔁 ADDING/REMOVING/CHANGING SUBJECT(S)
=======
## EMAIL FOR CONTACT FORM

You will change the email in this function to the email you would like responses from the form to be sent to. This is located in the contact.php file. The email currently in place is `szy17604@boofx.com`
`if ($success == false) {`
`//This user was not verified by recaptcha.`
`echo "Recaptcha Verification Failed";`
`} else if ($success == true) {`
`//This user is verified by recaptcha`
`if (mail("szy17604@boofx.com", $subject, $Body, $headers)){`
`//send successful`
`echo "Recaptcha Success, Mail Sent Successfully";`
`}else{`
`//send failure`
`echo "Mailing Failed";`
`}`
`}`

## ADDING/REMOVING/CHANGING SUBJECT(S)
>>>>>>> 1593df4199a7b72e3e387db372fb9401fc476abf

There is a section marked where you can edit the subject titles for the emails on the `index.html` file. You can use the following code to add more options and as an outline for how to label them:

`<option value="option-value">DISPLAY OPTION</option>`
