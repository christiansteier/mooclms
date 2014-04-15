.. _google_oauth_2.0_setup:

Google OAuth 2.0 Setup
=======================
Prior to Moodle 2.3, the Google Drive repository and Picasa web album repository and the Google Docs portfolio and Picasa portfolio could be used without any configuration or registration with Google. In April 2012, Google announced to web application developers that they would be deprecating the service which Moodle was using to communicate with Google and strongly advised developers to move away from it. As a response to this change with Google's service, Moodle switched to use a new system for communicating with Google called 'OAuth 2.0'. The OAuth 2.0 system provides a better security system and more friendly experience to Moodle users, though it requires some additional configuration in Moodle. 

Registering with Google
-------------------------
Each Moodle site now needs to be registered with Google in order to use the Google Drive, Docs or Picasa plugins. As part of the registration process, you will need to enter a URL (something like http://yourmoodlesite.org/admin/oauth2callback.php) which is provided on all Google Drive, Docs and Picasa plugins configuration pages in Moodle e.g. *Administration > Site administration > Plugins > Repositories > Google Drive*.

  1. Visit the `Google APIs Console <https://code.google.com/apis/console#access>`_ (or the new URL Google Cloud APIs Console) and sign into your google account. You will be asked to create a project if this is your first time using this form.
  2. Click the link on the left "API Access"
  3. Click the button 'Create an OAuth 2.0 client ID'
  4. Enter the branding information 'Product name' (i.e. the name of your Moodle site) and 'Product logo' (i.e. the URL of your site logo). By providing a descriptive name and link to distinct image then your users will know they are signing into the correct place.
  5. Click the Next button
  6. In 'Client ID Settings' select 'Web application' as application type.
  7. Click the '(more options)' link next to 'Your site or hostname' then in 'Authorized Redirect URIs' enter the URL (something like http://yourmoodlesite.org/admin/oauth2callback.php) from the plugin configuration page in Moodle, and leave the 'Authorized JavaScript Origins' field blank
  8. Click the button 'Create client ID' 

The Google Drive repository plugin also requires the Drive API to be enabled as follows:

  1. In the `Google APIs Console <https://code.google.com/apis/console#access>`_ click the link on the left "Services"
  2. Click the button opposite Drive API to turn it on 

Your site will then be registered with Google and you will be provided with a client ID and secret to configure all Google Drive, Docs and Picasa plugins.

**Tip:** If you have more than one Moodle site to register with Google, you can add an authorized redirect URI for each site in step 7. The same name and logo would then be displayed on the authorisation screen for each Moodle site. 

.. image:: _images/google_oauth1.png
Creating an OAuth Client ID

.. image:: _images/google_oauth2.png
Client ID settings

.. image:: _images/google_oauth3.png
Registered details

.. image:: _images/googledrive_repo2.png
Authorisation screen

Configuring the Google Docs and Picasa repositories
-----------------------------------------------------
  1. Go to *Administration > Site administration > Plugins > Repositories > Manage Repositories*.
  2. Activate the Google Docs and/or Picasa repositories by selecting 'Enable and visible' in the dropdown menu.
  3. Configure each repository by entering the client ID and secret. Make sure you don't include any white space in the text boxes.
  4. Save changes. 
  
Configuring the Google Docs and Picasa portfolios
---------------------------------------------------
  1. Go to Settings > Site administration > Plugins > Portfolios > Manage Portfolios
  2. Activate the Google Docs and/or Picasa portfolios by selecting 'Enable and visible' in the dropdown menu
  3. Configure each portfolio by entering the client ID and secret
  4. Save changes 

Once configured, Google will present Moodle users with a nice authorisation screen with your Moodle site name and logo for your users to authorise.

