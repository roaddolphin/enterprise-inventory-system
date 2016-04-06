This is a **hardware inventory** application that _stands the tests of time_.
It allows systems to be linked with others and keeps track of the applications running on them.

# Features #

  * very simple
  * XML files stored on a SQL database _all abstracted with DBI_
  * LDAP authentication _ActiveDirectory and RFC2307 LDAP databases supported_
  * mod\_perl2 based on top of Apache2 _really fast!_
  * system is OS agnostic
  * code follows modern [MVC](http://en.wikipedia.org/wiki/Model-view-controller) framework mentality and it was written from scratch (no framework used) on top of Class::DBI (to avoid [writing](http://www.perl.com/pub/a/2003/07/15/nocode.html) code)

# Requirements #

  * Apache + mod\_perl2
  * Template Toolkit
  * Class::DBI
  * Class::DBI::mysql
  * AppConfig _part of Template Toolkit_
  * Net::LDAP
  * XML::LibXML
  * XML::LibXSLT
  * Digest::MD5

The system already knows about **lshw -xml** and this is the preferred method to collect hardware information about a given host. However, you can always write your own collection script/application and your XML Stylesheet/schema to validate the data.

If you need write-commit access to this repository please do one of the following:
  * convince google to use Git, or
  * email the project administrator