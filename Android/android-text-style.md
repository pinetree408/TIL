make padding between text and textview's layout
```
android:paddingRight="10dp"
android:paddingLeft="10dp"
```

make underline at text in textview
```
TextView tv = (TextView) view.findViewById(R.id.tv);
SpannableString content = new SpannableString("Content");
content.setSpan(new UnderlineSpan(), 0, content.length(), 0);
tv.setText(content);
```
