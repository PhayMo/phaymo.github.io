ctrl+o: Command Pallete
ctrl+shift+a: Templates
ctrl+shift+q: Live Preview/Source
cmd+e: switch reading mode

# Dialogue Plugin:

### Advanced parameters


All parameters listed in the table above can be used to customize the dialogue.

#### Example code




```dialogue
left: Ingmar Bergman
right: Wong Kar-wai
titleMode: all
messageMaxWidth: 40%

< Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec tristique nunc, et pharetra sem.
< Nunc id auctor lectus, feugiat aliquet sem.

> Lorem ipsum dolor sit amet
> Ut nec efficitur mauris, a lacinia purus. Fusce nisi arcu, sollicitudin eget sodales sit amet, consectetur a lorem. Nam egestas tristique felis, sed suscipit nunc commodo nec.
```





### Change of parameters during a dialogue

Parameters can be modified during the dialogue (the change is applied to all following messages).

#### Example code



```dialogue
left: Ingmar Bergman
right: Wong Kar-wai

< Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec tristique nunc, et pharetra sem.
< Nunc id auctor lectus, feugiat aliquet sem.

> Lorem ipsum dolor sit amet
> Ut nec efficitur mauris, a lacinia purus. Fusce nisi arcu, sollicitudin eget sodales sit amet, consectetur a lorem. Nam egestas tristique felis, sed suscipit nunc commodo nec.

left: Sion Sono

< Nulla condimentum orci quis enim iaculis, ut congue turpis semper. Donec mattis elit vitae risus molestie vestibulum.
< In laoreet aliquet neque, eget tempus massa congue ut.
```

### Dialogue with delimiter


Use the `delimiter` (or shorter `-`) command to add a delimiter into the dialogue.

#### Example code



```dialogue
left: Ingmar Bergman
right: Wong Kar-wai

< Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec tristique nunc, et pharetra sem.
< Nunc id auctor lectus, feugiat aliquet sem.

delimiter

> Lorem ipsum dolor sit amet
> Ut nec efficitur mauris, a lacinia purus. Fusce nisi arcu, sollicitudin eget sodales sit amet, consectetur a lorem. Nam egestas tristique felis, sed suscipit nunc commodo nec.
```





### Dialogue with comments



Comments can be added into the dialogue with `#` prefix (see example below). The comment must be exactly one paragraph. Max width of the comments can be modified with the `commentMaxWidth:` parameter.

#### Example code



```dialogue
left: Ingmar Bergman
right: Wong Kar-wai

< Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec tristique nunc, et pharetra sem.
< Nunc id auctor lectus, feugiat aliquet sem.

# Lorem ipsum dolor sit amet

> Lorem ipsum dolor sit amet

# Vivamus nunc orci, aliquet varius rutrum et, pulvinar vitae nunc. Pellentesque a consequat ipsum.

> Ut nec efficitur mauris, a lacinia purus. Fusce nisi arcu, sollicitudin eget sodales sit amet, consectetur a lorem. Nam egestas tristique felis, sed suscipit nunc commodo nec.
```
