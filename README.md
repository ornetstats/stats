# OrNetStats

OrNetStats uses [onionoo.torproject.org](https://onionoo.torproject.org) data to generate statistics.
Statistics are generated on a daily basis.
For autonomous system and country stats you can use [compass.torproject.org](https://compass.torproject.org)

## Main Operators

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

* [Main Exit Operators](https://raw.githubusercontent.com/ornetstats/stats/master/o/main_exit_operators.txt)
* [Main Guard Operators](https://raw.githubusercontent.com/ornetstats/stats/master/o/main_guard_operators.txt)
* [Main Operators based on consensus weight](https://raw.githubusercontent.com/ornetstats/stats/master/o/main_operators_by_cw.txt)
* [Main non-Linux Operators](https://raw.githubusercontent.com/ornetstats/stats/master/o/main_non_linux_operators.txt)

* [Potentially dangerous groups](https://raw.githubusercontent.com/ornetstats/stats/master/o/potentially_dangerous_relaygroups.txt)
  * "dangerous" in the sense that a tor client might has a chance to use more than one of these relays in a single circuit at the entry and exit position
  * these relays are aggregated based on contact information
  * if their groupsize is bigger than their effective family size and they are operated in more than one /16 network block they are listed
  * this list might contain false-positives (contact information is not authenticated)

## Version Distribution

* [Major Version Distribution](https://github.com/ornetstats/stats/blob/master/o/major-version_share.txt)
* [Detailed Version Distribution](https://github.com/ornetstats/stats/blob/master/o/version_share.txt)
* [CVE-2016-8860 affected operators](https://github.com/ornetstats/stats/blob/master/o/cve-2016-8860.txt)

## OS Distribution

* [OS Distribution](https://github.com/ornetstats/stats/blob/master/o/os_share.txt)

## Stats on measured and recommended flag

* [What portion of the network runs not a recommended version?](https://github.com/ornetstats/stats/blob/master/o/recommended_version_share.txt)
* [What portion of the network is not measured?](https://github.com/ornetstats/stats/blob/master/o/measured_share.txt)
* [Unmeasured relays](https://raw.githubusercontent.com/ornetstats/stats/master/o/unmeasured_relays.txt) (new or re-appearing relays are expected to be unmeasured)
