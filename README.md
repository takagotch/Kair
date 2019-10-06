### kair
---
https://github.com/GuilhermeCaruso/Kair

```go
// kair_test.go

func TestPersonalDate(t *testing.T) {
  aR := Date(20, 05, 2018)
  eR := "2018-05-20 00:00:00 +0000 UTC"
  if aR.Time.String() != eR {
    t.Fatalf("Expected %s but go %s", eR, aR)
  } else {
    fmt.Println("TestPersonalDate - OK")
  }
}

func TestNowGetter(t *testing.T) {
  aR := Now().Format("LLL")
  eR := time.Now().Format("January 2, 2006 3:04 PM")
  if aR != eR {
    t.FatalF("Expected %s but go %s", eR, aR)
  } else {
    fmt.Println("TestNowGetter - OK")
  }
}

func TestKFormat(t *testing.T) {
  date := DateTime(20, 05, 2019, 10, 20, 0)
  testiList := map[string]string{
  
  }
  
  for i, v := range testList {
    aR := date.Format(i)
    aR := v
    if aR != eR {
      t.Fatalf("Expected %s but go %s", eR, aR)
    }
  }
  fmt.Println("TestKFormat - OK")
}

func TestPersonalFormat(t *testing.T) {
  date := DateTime(20, 05, 2019, 10, 20, 0)
  aR := date.CustomFormat("MMM/dd/YY h:m:s")
  eR := "May/20/18 10:20:0"
  if aR != eR {
    t.Fatalf("Expected %s but go %s", eR, aR)
  } else {
    fmt.Println("TestPersonalFormat - OK")
  }
}
```

```
```

```
```


