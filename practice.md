
create file state.txt with content
```
Arunachal Pradesh
Assam
Andhra Pradesh
Bihar
Chhattisgrah
```

Put parentheses around each item using `sed`

```
sed -E 's/(.*)/"\1"/g' state.txt
```

Expected output

```
"Arunachal Pradesh"
"Assam"
"Andhra Pradesh"
"Bihar"
"Chhattisgrah"
```


