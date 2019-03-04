This file is a template implementation report for WebSub subscribers. Copy this file to a new .md file and change the name to `HUB-project-name.md`, your project name (lowercase with hyphens between words). Fill out the information based on the details of your implementation. It's okay to not check all the boxes, we are more interested in knowing how much of the spec is implemented than getting everyone to tick every box. When you are finished, submit a pull request or link to your file in a [new issue](https://github.com/w3c/websub/issues).

For items that have a number next to the checkbox, the number corresponds with the test number on websub.rocks. You can use that tool to check whether you support the feature properly. To mark a statement as true, add an x between the brackets, e.g. [x]. If the statement does not apply to your implementation, use [na] and add a sentence explaining why it does not apply.

Delete the section above when filling out your copy of this file.

Implementation Home Page URL:http://pubsubhubbub.appspot.com/ 

Source code repo URL(s) (optional):
* [x] 100% open source implementation

Programming Language(s): 

Developer(s): [Name](https://you.example.com)

Answers are:
* [x] Confirmed via websub.rocks (for applicable results)
* [ ] All results are self-reported

## Subscription

* [x] 100: Supports subscriptions with `hub.mode`, `hub.topic` and `hub.callback`
* [x] 101: Supports subscriptions with `hub.mode`, `hub.topic`, `hub.callback` and `hub.secret`
* [x] 102: Ignores unrecognized parameters in the subscription request
* [x] 103: Allows subscribers to re-request active subscriptions before they expire
* [x] 104: Supports unsubscription requests
* [x] 1xx: Sends a properly formatted verification request for subscribing and unsubscribing
* [x] Allows subscribers to request a specific lease duration
  * If not, then describe the default lease duration issued, or other specifics here

(1xx denotes that you can can use any of the 100-104 tests to confirm this feature)

## Distribution

* [x] 100: Sends a notification with a matching content-type of the topic URL
* [x] 100: Sends a notification with the full contents of the topic
* [x] 101: Sends a notification with a valid signature
  * Please select the signature method(s) that the hub uses to sign requests
  * [x] sha1
  * [ ] sha256
  * [ ] sha384
  * [ ] sha512
* [x] Sends only a diff of the topic URL for Atom or RSS feeds
