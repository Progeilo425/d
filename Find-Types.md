There are 4 main find types you can find within AdvancedChat.

- Literal
- Upper Lower
- RegEx
- Custom

## Literal

Literal searches for exactly  what the search string is, character-for-character. Here's an example:

**Find String:** `Hello`

**Matches:** `Hello`, `Hello how is your day`, `hi. Hello!`

**Doesn't Match:** `hello`, `hi`, `HELLO`, `this is a phrase`

## Upper Lower

Upper lower is like literal, but ignores case.

**Find String:** `Hello`

**Matches:** `Hello`, `HELLO! how is your day`, `hi. hello!`, 'hello good sir'

**Doesn't Match:** `hi`, `this is a phrase`

## Regular Expression (RegEx)

RegEx takes in a [Regular Expression](https://en.wikipedia.org/wiki/Regular_expression) and matches based off of that. While confusing to learn, RegEx is a powerful tool to match complex strings. A really good website to help test RegEx is [regex101](https://regex101.com/). To learn RegEx there are many resources online, one recommended is [Fireship's video](https://www.youtube.com/watch?v=sXQxhojSdZM).

## Custom

Each module can add a custom filter and add powerful find types. To access them, set the find type to custom, and then the find string to their specific name. Different custom find types can have options appended past their name.

Example:

**FindType:** Custom

**FindString:** `profanity`

This will then match any profane words as defined in `config/advancedchat/swear_words.txt`

The following are the base custom find types.

### Profane Words

Usage: `profanity` 