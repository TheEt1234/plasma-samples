# Plasma samples
This silly project hasn't been endorsed/developed by KDE in any way
i dunno if plasma is trademarked or not


## Naming scheme
- `ocean_<whatever>` - came from ocean sound theme
- `oxygen_<whatever>` - came from oxygen sounds
- the sounds itself also have `word1-word2-word3` naming scheme
  - Yes it looks strange, but you can use `"dialog-warning".bank("oxygen").s()` for example, so its worth it

## Included sounds
- https://invent.kde.org/plasma/oxygen-sounds
- https://invent.kde.org/plasma/ocean-sound-theme

And their licenses

## Use
```es
samples('github:TheEt1234/plasma-samples/refs/heads/main')
```


## Example
```js
// "You can make something more creative than this" @license CC0
samples('github:TheEt1234/plasma-samples/refs/heads/main')

$: s("dialog-error*4").bank("oxygen").delay(.2).dec(.8)

$: note("a")
  .s("dialog-error").bank("ocean")
.delay(.2)
```
