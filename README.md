# DRRT JSON Enforcer
This mod is made for the Debris Regional Reassembly Tournament series.
**EXTREMELY SIMPLE MOD** that changes a single cvar:
```
kWriteJSON = 1
```
This causes Reassembly to output JSON files instead of Lua files in most
situations. Most importantly, this mod makes Reassembly export ship and fleet
files in the JSON format. This is useful if you need to work with Reassembly
ship files in a scripting language, as most appear to have tools for reading
and writing to JSON files easily. 

Reassembly can read JSON or Lua formatted files **with or without** the mod
enabled. This mod only declares the format that Reassembly will write files
with.

In order to generate fleet files for the Qualifications, DRRT uses a Python
script that loads ship files into Python data structures. The ubiquity of the
JSON format makes this terribly easy, as Python already has sophisticated tools
for working with JSON. If all ship files are in the JSON format, loading them
in as dicts is not challenging whatsoever.

JSON format export of Terran Interceptor featured in preview image.
