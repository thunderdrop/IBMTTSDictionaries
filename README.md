# IBMTTSDictionaries
For use with ECI.DLL.
## Description
This is a community project for modifying pronunciation dictionary files, used with the IBMTTS (ETI Eloquence) driver (not provided). You will either need the ECI library, or something which incorporates it, and    supports the loading of custom dictionaries, such as a screen reader addon or text to speech program.
## Usage
If you are using an NVDA addon or similar which incorporates this dictionary already, you do not need to do anything to make your existing dictionary work.

Otherwise, to update or install: copy all contained files with a .dic  extention to the location of the driver binary, usually ECI.DLL.
In NVDA, this is quite often in a folder called "eloquence" or "ibmtts" in the synthDrivers folder of the addon you installed.

If you are wrapping this driver yourself, you will need to implement it such that your implementation can load and parse these files (not documented here).
### hyphenated words support
The main dictionary has support for words containing hyphens. By default, however, NVDA will block the hyphen from being sent to the synthesizer. To make this work as intended, open NVDA's punctuation/symbol prununciation settings under preferences, type dash, and set the level to always or only below symbol's level. The default level should be at most, which if you set to the only below setting will cause the dash to reach the driver unchanged at the some and none levels, but to be spoken at the most level.
## Contributing
Contributions will be factored into a new stable version of the dictionaries, to be released on the first day of every month.

feel free to make as many pull requests as you wish, with your modifications or additions to the dictionaries. Pull requests must consist of valid phonemic syntax for American English.

If you wish to contribute without making a pull request, comment on the Submissions issue for the present month with your changes, with optional syntax, phonetic pronunciation guide, or IPA transcription. You will find the relevant issues open and awaiting your input!

Pronunciation tends toward General American for most words, though IBMTTS itself has an accent more specific to middle and northern New England. Names and other proper nouns may require some discussion.

## Credits
These files are maintained by [amirsol81](https://github.com/amirsol81),   [x0](https://github.com/ultrasound1372), and [thunderdrop](https://github.com/thunderdrop), with contributions from many.

NO ownership of the IBMTTS driver and/or dependencies is implied or should be inferred.
