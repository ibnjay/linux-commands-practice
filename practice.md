
create file state.txt with content
```
Arunachal Pradesh
Assam
Andhra Pradesh
Bihar
Chhattisgrah
```

<b>Put parentheses around each item using `sed` </b>

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



<b>Replace desh with land using `sed` </b>

```
sed -E 's/desh/land/g' state.txt
```

Expected output

```
Arunachal Praland
Assam
Andhra Praland
Bihar
Chhattisgrah
```

