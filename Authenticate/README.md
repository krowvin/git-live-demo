# How to Authenticate to GitHub 
*For use with Command Line, details can be found [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic)*

## Option 1: Manually Create the Key
1. Login to [GitHub](https://github.com)
2. Open Settings:
   1. Click your user portrait at the top right of the window: ![User Portrait](images\portrait.png)  
   2. Click Settings  
   ![User Settings](images\user_settings.png)
3. Scroll to the bottom and click \<Developer Settings\>
   ![Dev Settings](images\dev_settings.png)
4. Click "Personal access tokens"
5. Click "Tokens (classic)"  
![Classic Token](images\token_classic.png)
6. Click "Generate new token" dropdown
7. Click "Generate new token (classic)" in the dropdown menu
![Gen Token](images\generate_token_classic.png)
8. **Type** a note to future you about what this token is for, in our case "windows command prompt"  
and **check the boxes** for the scope(s) you want this token to have access to:  
![Scope](images\scope.png)
9. Click "Generate token"  
![Gen Token](images\generate_token.png)
10.  Click the copy button to copy your key  
![Copy your key](images\copy_key.png)
11.  Run your git command again to push/clone from remote
12.  When prompted, click the "token" tab and paste int he token you copied from step 10  
![token_auth](images\token_auth_2.png)

You are done! you should now have a cached session on your system for authenticating with github. You can revoke this token in the menu (Step 3/4 at any time)  

## Option 2: Login via prompt
1. If you try to clone a repo and/or need to authenticate newer versions of git can prompt you for your github login. Enter your credentials here and it will generate the key for you!  
![Sign in](images\sign_in_user.png)  



**Thank you to Theresa for the screenshots on setting up a new user!**