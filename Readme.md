ever wanted to google from your terminal?

just put this in your terminal
```bash
echo 'function gg {
  string="$*";
  search="${string// /+}";
  googleurl="https://www.google.com/search?q=$search";
  open $googleurl;
}
alias gg="gg"' >> ~/.bashrc; source ~/.bashrc;
```

then you can google using `gg` <whatever you want here seperated by spaces.>

## Try it out!
example: `gg 'github michaeldimmitt'`
