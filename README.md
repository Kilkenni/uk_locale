# uk_locale
##Update:

The overrides method allows any mod to provide a translation for any other mod.

##About
An ongoing ukrainian translation for Stonehearth core. Very much a WIP. The curator on Stonehearth Discourse platform is MelOzone.

##How it works:

For testing put all te files in the separate folder inside your Stonehearth's mod folder. Then choose Ukrainian in the game options.

##How to translate en.json:

Only translate strings that come after a ':'' in the json file. You can more easily view the json on a website such as http://codebeautify.org/jsonviewer
Do not modify the strings that come on the left side of a ':'
Also, do not modify strings that are surrounded by brackets '[' or ']'

Example:
  ````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "chasing [name(data.target)]",
  ````

Here, the string that needs to be translated is "chasing [name(data.target)]"
Note, DO NOT translate the "[name(data.target)]" portion. This is a special string replacement. The name of the target will replace "[name(data.target)]" in the game.

EX: If a hearthling is chasing a goblin named "Jib", the game will replace "[name(data.target)]" with "Jib" and the final string will read: "chasing Jib"

The replacement is character sensitive, so do not change whether the string is upper or lower case, and do not replace any of the string with a different key. It is best
to copy and past the special portion into your translated text.

You can move "[name(data.target)]" around to different locations within the string.

The japanese translated file might show something like this:<br>
  ````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "[name(data.target)]を追う",
  ````

The Chinese file might look like:<br>
  ````
  "ai": {
   "actions": {
      "status_text": {
         "chase_entity": "追逐[name(data.target)]",
  ````
