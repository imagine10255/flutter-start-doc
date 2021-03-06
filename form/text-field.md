---
description: TextField
---

# TextField

![&#x8F38;&#x5165;&#x6846;&#x793A;&#x610F;&#x5716;](../.gitbook/assets/cleanshot-2021-07-26-at-15.05.08-2x.jpg)

表單的文字輸入框欄位  
可使用 TextFormField

### 使用方法

```text
TextFormField(
    controller: widget.controller,
    onChanged: _onChange,
    onTap: widget.onTab,
    enabled: !widget.disabled,
    obscureText: widget.isPassword,
    decoration: InputDecoration(
      icon: widget.beforeIcon != null ? Icon(widget.beforeIcon!, size: 30, color: kGreyColor) : null,
      border: OutlineInputBorder(
        borderRadius: BorderRadius.circular(0),
      ),
      helperText: widget.desc,
      helperMaxLines: 5,
      labelText: widget.label,

      suffixIcon: afterIconCode != null ? GestureDetector(
        child: Padding(
          padding: EdgeInsets.all(8),
          child: Icon(afterIconCode),
        ),
        onTap: afterIconOnPress != null ? afterIconOnPress: null,
      ): null,
    ),
    validator: (value) {
      if(widget.validator?.isRequired == true){
        if (value == null || value.isEmpty) {
          return 'Please enter some text';
        }
      }
      return null;
    },
    // onSaved: widget.onChange <~ 好像用不到
);
```

 





