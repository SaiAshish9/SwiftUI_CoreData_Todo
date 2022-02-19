```
guard let url = URL(string: self.link), UIApplication.shared.canOpenURL(url) else {
  return
}
UIApplication.shared.open(url as URL)
```

```
@Published public var themeSettings: Int = UserDefaults.standard.integer(forKey: "Theme") {
  didSet {
    UserDefaults.standard.set(self.themeSettings, forKey: "Theme")
  }
}
```

```
self.theme.themeSettings = item.id
UserDefaults.standard.set(self.theme.themeSettings, forKey: "Theme")
self.isThemeChanged.toggle()
```
