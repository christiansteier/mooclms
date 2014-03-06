.. _paypal:

PayPal
=======
**Location:** PayPal edit settings link in *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*

The PayPal enrolment plugin allows you to set up paid courses. The plugin has to be enabled by the site administrator (see Enrolment plugins)and then added to the course by an administrator or manager. You can then set an individual price for your course if needed. 

Course settings for PayPal
---------------------------

Checking you have Paypal in your course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * In a course, go to *Administration > Course administration > Users > Enrolment methods*
    * If you do not see PayPal, use the pull down menu "Add method" and select PayPal. 
    * Make sure PayPal has its "eye" opened: 

Setting a price for your course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * In *Administration > Course Administration > Users > Enrolment methods*, click the edit/hand/pen icon to the right of the Paypal option.
    * Give a name to this enrolment method if you wish in "Custom Instance name". (You don't have to!)
    * Ensure that "allow Paypal enrolments" is set to "yes"
    * In "Enrol cost", type in the cost of your course and in "Currency" choose your currency. 

**Note:** In Moodle 2.5 onwards, all Paypal-supported currencies are available.

    * Usually you would leave the "Assign role" as "student" unless you have a very special reason for allowing your users to enrol as, say, editing teachers etc
    * Choose an enrolment period and/or start/end dates if desired.
    * Click the "Save changes" button. 

What the new user sees
^^^^^^^^^^^^^^^^^^^^^^^^
When a new user clicks on your course link, having made a login to your Moodle, they will see the following screen, inviting them to go to PayPal to purchase access to your course: 
    

Admin settings
----------------
    1. If you wish to allow users to make their own accounts on your site then set up Email based self registration
    2. Go to *Administration > Site Administration > Plugins > Enrolments > Manage enrol plugins* and enable (open the "eye" of Paypal)
    3. Click the blue Settings link to the right of the PayPal enrolment link. Here are the default settings and default settings for new instances in a course:
         1. Add the email of your Business PayPal account. The email settings are case sensitive and must exactly match that in PayPal.
         2. Choose whether to notify students/teachers/admin.
         3. Choose whether (or not) to allow the Paypal enrolment plugin by default in new courses
         4. Choose a default cost and currency. (This may be overridden in individual courses)
         5. Choose a default role assignment. (This means the role that a new user will automatically be given in a course when they purchase access. Usually this would be "student" unless you have a special reason for choosing another role.) This may be overridden in individual courses.
         6. Choose the default enrolment period. This may be overridden in individual courses. 

What to set up in Paypal
--------------------------
   * Setup your PayPal account at paypal.com 

      1. Create a Paypal account
      2. Not required but recommended for selling: Upgrade your account to "Premier" status and get "Verified"
      3. Set the Encoding to UFT-8. In Paypal, go to "Profile > Language Encoding" (under the Selling Preferences column) and set your website's language (like select "Western European Languages (including English)" as it is the only English version). Then click on the "More Options" button and set the Encoding to "UTF-8", select "Yes" to use the same encoding for data sent from Paypay to you, and save.
      4. Optionally setup IPN in Paypal to interact with Moodle. Log into Paypal, go to "Profile > Instant Payment Notifications (IPN)”, click "Turn On IPN", click the "Edit settings" and enter a URL that references your IPN file in your Moodle installation (for example: http://<domain name>/moodle/enrol/paypal/ipn.php) 

What the user sees
--------------------
   * If you have allowed users to create their own accounts then when they click to login, they will be presented with a screen Is this your first time here? It will give them instructions for making an account (which may be customised in the authentication common settings in *Administration > Site administration > Plugins > Authentication > Manage authentication*) and once their account is confirmed via email they can click on a course which can be purchased and pay for it via Paypal. PayPal courses will have a dollar sign icon next to them:
   * Once payment is made both the user/student and the teacher/admin should have received emails from Paypal confirming the purchase. 

Changing the dollar symbol
----------------------------
The default currency symbol for Paypal is a dollar sign. If you are using GBP or Euros or another currency, you can change this by creating your own customised icon with your choice of currency. Make it 16x 16 pixels and call it icon.gif Upload your new icon via FTP to your moodle directory>enrol>paypal>pix. Your icon.gif will override the dollar sign. Make sure you refresh your page to be sure of the changes. 












