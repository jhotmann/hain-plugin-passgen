# How it works
Type /pass [some passphrase here] into Hain. The passgen plugin takes your input string,
appends a unique salt string to it, and then generates a hash. The resulting hash is then
base91 encoded so that it uses all uppercase and lowercase letters, numbers, and standard
symbols.  A subset of 15-100 (default is 40 and can be changed in preferences) characters
is picked from the base91 encoded hash and then placed in your clipboard to be pasted into
a password field.

Every time you use the same input string, you will get the same result from the passgen
plugin. This allows you to use an easy to remember passphrases to generate lengthy,
complicated passwords that no one can reproduce unless they know your passphrase, salt,
and method of generating passwords.

# Installation
1. Install Hain if you haven't already https://github.com/appetizermonster/hain
2. Type `/hpm install hain-plugin-passgen` into Hain
3. Type `/pass` and hit enter in Hain to go to the preferences screen. Paste the randomly generated salt (or a custom salt) into the Salt field
4. Done. You can now generate passwords.
