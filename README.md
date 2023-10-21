```driver.get('chrome://extensions/')
    js_code = "return document.querySelector('extensions-manager').extensions_.map(({id, name}) => ({id, name}))"
    ext_id = driver.execute_script(js_code)[0]['id']
    driver.get(f'chrome-extension://{ext_id}/popup.html')
```
    
