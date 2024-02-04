## Features

The editor offers the following <b>options</b>:

- [x] **Bold**
- [x] *Italic*
- [x] <u>Underline</u>
- [x] Different Heading

- [ ] 
## How to use ?

```
@Composable
fun Sample() {

        val context = LocalContext.current
        
        val state = remember {
            val input = /* YOUR INPUT */
            RichEditorState.Builder()
                .setInput(input)
                .adapter(JsonEditorParser())
                .build()
        }

        RichEditor(
                state = state,
                modifier = Modifier
                    .fillMaxWidth()
                    .weight(1f)
                    .border(1.dp, Color.Gray)
                    .padding(5.dp)
            )
    
}
```
