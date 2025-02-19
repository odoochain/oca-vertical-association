====================
Membership extension
====================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:d30c155b2d6127e8e0648c7440ca4401bb187ee48be803e94d7452934881610c
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fvertical--association-lightgray.png?logo=github
    :target: https://github.com/OCA/vertical-association/tree/16.0/membership_extension
    :alt: OCA/vertical-association
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/vertical-association-16-0/vertical-association-16-0-membership_extension
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/vertical-association&target_branch=16.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module extends Odoo's membership management with the following features:

* Membership category
* Membership lines editable
* Do not calculate membership state from invoice status
* Start date of last membership period
* Partner's with member lines can't be deleted.
* When a partner has an associated member there is the option to make member
  start date independent from the associated member one so joining dates can be
  tracked for those members.
* Adds a category for Membership management security group so a user with only
  that permission can access to the membership menu.

**Table of contents**

.. contents::
   :local:

Configuration
=============

Users can define membership categories in Association > Configuration > Membership Categories
Then go to membership products and set a category to each one.

Usage
=====

Membership categories allow to classify memberships by types, allowing a
partner to be member or not of the different categories. For example, if you
have several levels of partnership (Starter, Silver, Gold) and one product
for each one, then partners who buy Silver product will have Silver membership
category. Afterwords, you can filter Silver members.

Membership lines are created when a membership product is invoiced, like in
Odoo standard version. But now users can create a new membership line without
creating an invoice.

Also, users can edit membership line dates and state even if an invoice is
not related with it.

You will see a general membership status at partner level that specifies if
it's a member of any category or not, and also a detail status per
membership category.

To make member start date independent from the associated member one, check the
option *Adhered member* in the membership tab of the partner who is associating.
A start date will now be available to edit.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/vertical-association/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/vertical-association/issues/new?body=module:%20membership_extension%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Tecnativa
* Onestein

Contributors
~~~~~~~~~~~~

* Antonio Espinosa <antonio.espinosa@tecnativa.com>
* Pedro M. Baeza <pedro.baeza@tecnativa.com>
* David Vidal <david.vidal@tecnativa.com>
* Rafael Blasco <rafael.blasco@tecnativa.com>
* Luis M. Ontalba <luis.martinez@tecnativa.com>
* Alberto Martín Cortada <alberto.martin@guadaltech.es>
* Andrea Stirpe <a.stirpe@onestein.nl>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/vertical-association <https://github.com/OCA/vertical-association/tree/16.0/membership_extension>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
