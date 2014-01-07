Secure Calls
============

Phone calls made over mobile telephone networks were designed to have some forms of protection in order to help prevent call interception, user impersonation and tracking of users by a third party. However, mobile phone networks were and are not designed to prevent the mobile phone operator or other 'trusted' parties connected to their network from carrying out interception, impersonation and tracking. For example, the widely deployed [A5/1](https://en.wikipedia.org/wiki/A5/1) stream cipher, which is used to provide over-the-air communication privacy in the GSM cellular telephone standard, has been broken for many many years ([30C3: Mobile Network Attack Evolution](http://media.ccc.de/browse/congress/2013/30C3_-_5449_-_en_-_saal_1_-_201312271715_-_mobile_network_attack_evolution_-_karsten_nohl_-_luca_melette.html)). In addition to these weaknesses, phone calls are not encrypted end-to-end and telephone providers are increasingly forced to give governments and law enforcement bulk access to your calls and data about your calls [e.g. the NSA's MAINWAY database](https://en.wikipedia.org/wiki/MAINWAY) contains metadata for hundreds of billions of telephone calls made through the four largest telephone carriers in the United States.

There are well known passive interception and active interception methods all of which are currently used against GSM networks and their users. [Read more](https://gsmmap.org/assets/pdfs/gsmmap.org-country_report-Germany-2013-12.pdf) about the current state of Germany's GSM network security as of December 2013.

Anyone with enough interest and a modest amount of money can buy the equipment to intercept calls. The cheapest GSM interceptor devices cost as little as $9. More sophisticated, 'active interception' techniques require more expensive equipment.


Active intercept (source: https://gsmmap.org/assets/pdfs/gsmmap.org-country_report-Germany-2013-12.pdf, pending permission from author for usage)
----------------
Attacks through fake base stations can be prevented to different degrees, based on what the fake base station is used for:

*Location finding*: In this attack scenario, a phone is lured onto a fake station so that the phone’s exact location can be determined. This scenario occurs independent from the phone network and hence cannot be prevented through network protection measures.

*Outgoing call/SMS intercept*: A fake base station can proxy outgoing connections. In this attack, the network is not necessarily required, so no protection can be achieved from outside the phone.

*Encrypted call/SMS intercept*: Modern fake base stations execute full man-in-the-middle attacks in which connections are maintained with both the phone and the real network. Networks can make such active attacks more difficult with a combination of two measures: 
  * First, by disabling unencrypted A5/0 calls.
  * Secondly, by decreasing the authentication time given to a the attacker to break the encrytion key. This timeout can be as much as 24 seconds according to GSM standards. All of the networks use encryption in all call and SMS transactions; however, the GSMmap currently lacks data to decide whether the networks would accept
unencrypted transactions as well.

Centralised or proprietary systems like Skype also encrypt calls but have built in backdoors for secret services and governments and are at the behest of their owner (in Skype's case Microsoft).

A solution to this problem is to make encrypted calls using Voice over IP (VoIP) through an Internet connection. Both WiFi or mobile data networks can be used: cracking the GSM or Wireless password will not mean that your call can be intercepted.

Android has a wider range of open source VoIP software whereas options for Apple users is limited. This is, in part due to the fact that the Apple AppStore licensing model prohibits distribution of software released under the *General Public License* (which applies to approximately 60% of all open source software released). The GPL is very popular in the security and networking community.

At the time of writing iPhone users only have proprietary options available for purchase, like *Groundwire* [http://www.acrobits.cz/11/acrobits-groundwire-for-iphone](http://www.acrobits.cz/11/acrobits-groundwire-for-iphone). **Warning: as it is not open, the security of Groundwire cannot be assured!**

Android users head over to the section **Call Encryption** to get started making secure VoIP calls.
