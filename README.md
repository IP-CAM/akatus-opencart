<p align = "left">
    <img src = "https://site.akatus.com/wp-content/uploads/2012/12/logo.gif" alt = "akatus" title = "akatus" />
</ p>

# Akatus module for OpenCart (1.5.3.1 or higher)

__ImPortant: __ There are two versions available for this module.
By default the download version is without One Step Checkout.
If you want to use the version with One Step Checkout Click on the link: https://github.com/akatus/akatus-opencart/archive/one_step_checkout.zip

## Installation

__Actention: __ Make a complete backup of your store's files and database before starting the installation.
             
__The module requires installation of vqmod__


* Open the compressed file and extract all directories in the root of your OpenCart store, overwriting existing files and directories.

* Run only once the file "akatus_db_install.php", accessing it through http://sualoja.com.br/akatus_db_install.php. This file will create the status of
Shopping we need to update the payments. If everything works out, it will appear
The message "Akatus transaction status were successfully inserted" at the end of execution.

* Log in to the administration. Go to the Menu * Extensions >> Payments *. There will appear 3 new akatus - credit cards, banking bill and electronic transfer. Click the Install link, located on the right side of each of them and then in Edit.

## Settings

* __Name__ - Add a name to be displayed at checkout.

* __Status default requests__ - Select the status "awaiting payment"

* __Zona__ - Select the payment zone where the module should be displayed. Keep the "all zones" option.

* __OrDem__ - Enter the order in which this payment option should be displayed at checkout __ (integer) __.

* __ Parcelamento without interest until__ - inform how many installments you want to take on interest. In order for this option to work correctly, it is also necessary to change it in your
Akatus in * "My Account >> Payment Means" *. The default value is 1. __ * (credit card only) * __

* __Status__ - Select Active

## Account data akatus

* __Type__ - Production or Sandbox (for testing)

* __A-mail account__ - Akatus account registration e-mail

* __Token NIP__ - Code Generated in the Akatus Account Panel (Integration Menu> Security Keys)

* __Api Key__ - Code generated in the Akatus account panel (Integration menu> Security keys)

* __ Public Token__ - Code generated in the Akatus account panel (Integration menu> Security keys)

* Maximum number of parcels__ - Enter as many
PLOTS The user can split their purchases. The default is 12 installments, and the minimum portion value will always be 5 reais.
__ * (credit card only) * __

## Instant payment notification (NIP)

To receive changes notifications in transaction status is required:

1. Access the menu * Integration >> Notifications *, within your Akatus account.
2. Enable notifications and insert the URL in the default: http://www.sualoja.com.br/akatus/retano.php

Click Save.

__Oping: __ It is interesting to use HTTPS for NIP, however it is necessary that the server is correctly configured and with valid SSL certificate.


## Discount Setup

The discount option is only available for ticket and TEF. Enter the respective payment options and perform the configuration.
We remind you that the field only accepts percentage.


## Showing the discount amount at checkout

To show the discount amount at checkout between: * Extensions >> Order Totals * and activate the Akatus Discount Docket and Akatus Discount TEF options.
