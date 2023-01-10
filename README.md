# Registration-form
Registration form by using html and CSS
#html code

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Registration portal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Welcome to our Registration Portal</h1>
    <h2>Registration Form</h2>
    <p>Please fill out this form with the required information</p>
    <form method="post" action='https://register-demo.freecodecamp.org'>
        <fieldset>
            <label for="first-name"> Enter Your First Name: 
                <input id="first-name" name="first-name" type="text" required/>
            </label>
            <label for="last-name"> Enter Your Last Name: 
                <input id="last-name" name="last-name" type="text" required/>
            </label>
            <label for="email"> Enter Your Email Id: 
                <input id="email" name="email" type="text" required/>
            </label>
            <label for="new-password">Create a New Password: 
                <input id="new-password" name="new-password" type="password" pattern="[a-z0-5]{8,}" required />
            </label>
            <label for="new-password">Confirm Password: 
                <input id="new-password" name="new-password" type="password" pattern="[a-z0-5]{8,}" required />
            </label>
            </label>
        </fieldset>
        <fieldset>
            <label for="personal-account">
                <input id="personal-account" type="radio" name="account-type" class="inline" /> 
                Personal Account</label>
                <label for="business-account">
                    <input id="business-account" type="radio" name="account-type" class="inline" /> 
                    Business Account</label>
                    <label for="terms-and-conditions">
                        <input id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" class="inline" /> 
                        I accept the <a href="">terms and conditions</a>
                      </label>
        </fieldset>
        <fieldset>
            <label for="profile-picture">Upload a profile picture: 
                <input id="profile-picture" type="file" name="file" />
            </label>
            <label for="age">Input your age (years): 
                <input id="age" type="number" name="age" min="18" max="60"/>
            </label>
        <label for="referrer">How did you hear about our portal?
            <select id="referrer" name="referrer">
            <option value="">(select one)</option>
            <option value="1">Advertisement</option>
            <option value="2">YouTube Channel</option>
            <option value="3">By Friends or by Family Member </option>
            <option value="4">Others</option>
          </select>
        </label>
        <label for="bio">About Yourself:
            <textarea id="bio" name="bio" rows="3" cols="30" placeholder="I like coding on the beach...">
            </textarea>
          </label>
        </fieldset>
        <input type="submit" value="Submit" />
    </form>
</body>
</html>
