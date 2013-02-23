スライド内にあるコマンド一覧

```bash
git clone git@github.com:eiel/git-object-sample.git
cd git-object-sample.git
```

```bash
tree
```

```bash
tree .git/objects
```

```bash
echo "READMEを上書き" > README.md
git commit -a -m 'READEMを上書きしました'
cat README.md
```

```bash
ruby -rzlib -e 'puts Zlib.inflate(ARGF.read)'
```

```bash
cat .git/objects/a0/d74d48d61f95a874e30f8fb71bbd68506d0f6e  ruby -rzlib -e 'puts Zlib.inflate(ARGF.read)'
```

```bash
cat .git/objects/a0/d74d48d61f95a874e30f8fb71bbd68506d0f6e | ruby -rzlib -e 'puts Zlib.inflate(ARGF.read)' | od -c
```

```bash
cat .git/objects/a0/d74d48d61f95a874e30f8fb71bbd68506d0f6e | ruby -rzlib -e 'puts Zlib.inflate(ARGF.read)' | sha1sum
```

```bash
git cat-file -t a0d74
git cat-file -s a0d74
git cat-file -p a0d74
git show a0d74
```

```bash
git rev-list --all --objects
```

```bash
git cat-file -p 7dca985cea0d6e31591b46fe2610d5538dce466d
```
