.. include:: ../global.rst

Configuring Telegram for NEMS Notifications
===========================================

Telegram is a free chat service with an  supporting Push notifications
on Android and iOS.

NEMS Linux includes *notify_*\ :bolditalic:`host`\ *_by_telegram* and *notify_*\ :bolditalic:`service`\ *_by_telegram*.

It's fairly simple to setup, as long as you have your device (ie.,
smartphone) and a computer/laptop handy.

1) Install the free `Telegram app <https://telegram.org/apps>`__ on your
device.

2) Run the app and follow the simple on-screen prompts to activate a
Telegram account (it's free).

3) Create a new message and search for *botfather*.

.. figure:: ../img/screenshot_2019-08-19-19-28-48-089_org.telegram.messenger.png
  :width: 400
  :align: center
  :alt: Botfather

4) Click on the BotFather bot result, and then click *Start* at the
bottom of your app screen.

5) Click ``newbot`` and then type a name for your bot. *NEMS Linux* is
one idea.

6) Choose a username for the bot, which must end in the word *bot*. For
example, you could call it *mycoolbot*, *mycoolbot_bot* or
even *mycool_bot*. I might consider *BaldNerdNEMS_bot* as my bot
username.

7) If all went well, you will then receive an in-app notice that says
“Done. Congratulations on your new bot.” followed by some information.
In particular, you'll need to remember your bot name (created in the
step above) and the  token.

.. figure:: ../img/screenshot_2019-08-19-19-32-50-622_org.telegram.messenger.png
  :width: 400
  :align: center
  :alt: Botfather 2

8) Click *back* |back| followed by the hamburger menu |hamburger| then choose *New
Group*.

.. |back| image:: ../img/back.png
   :height: 2em

.. |hamburger| image:: ../img/hamburger.png
   :height: 2em 

9) Search for the bot you just created just as if it was a person, and
click it to add the bot to your new group.

.. figure:: ../img/screenshot_2019-08-19-19-41-44-985_org.telegram.messenger.png
  :width: 400
  :align: center
  :alt: New Group 200000

Click your bot's name from the search results, followed by the right
arrow |rightarrow| to proceed to the next screen.

.. |rightarrow| image:: ../img/rightarrow.png
   :height: 2em

10) Enter a name for your group and click the checkmark to save.

.. figure:: ../img/screenshot_2019-08-19-19-43-25-138_org.telegram.messenger.png
  :width: 400
  :align: center
  :alt: New Group

11) On a computer, open the  https://web.telegram.org/ and sign in with
the phone number you used to activate your Telegram account.

12) Click on the group chat you added your bot to and look at the
address bar. It will have a  such as
\https://web.telegram.org/#/im?p=\ **gXXXXXXXXX** - hold on to that info
(Chat ID: **gXXXXXXXXX**)

13) On your NEMS Server, open `NEMS
SST <../apps/nems-sst.html>`__ and add your
bot  Token and Chat ID to the Telegram Account Info section on
the *Notifications* tab.

14) Finally, open NEMS NConf and modify your Contacts (Contacts → Show →
Modify). Add notify_host_by_telegram and notify_service_by_telegram
appropriately. Save, and generate your Nagios Config.

.. figure:: ../img/telegram.png
  :width: 400
  :align: center
  :alt: Telegram

Thanks
to `baggins <https://forum.nemslinux.com/viewtopic.php?f=44&t=96&hilit=baggins>`__ for
contributing this feature and Vincenzo Di Iorio for assisting with this
documentation.
