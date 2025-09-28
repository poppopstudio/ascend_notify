# Ascend GovUK Notify installer

This recipe will install the GovUK Notify and Key contrib modules, and set up
keys & config overrides for those keys, to prevent sensitive data being present
in database exports. It also sets GN to be the default sender for system emails.
It assumes you have access to the project root to create folders & files, and
that you are okay with using a folder called 'keys' to store these files and
values.

## Installation

- Read the GovUK Notify module installation instructions, being mindful that you
will be doing things a bit differently because of this recipe.
- Create a 'keys' folder in project root & create text files to store them.
  - mkdir keys && cd keys && touch govuk_api.key govuk_email.key govuk_sms.key
- Place the API key values into the relevant files.
- Secure the folder & files as is pertinent to your setup.
