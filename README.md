# COVID DATA ERROR

This is the link to my website - [https://abd360superman.github.io/coviddata-error/]

## ERROR

If you navigate to js/coviddata.js inside the renderTable() function, you will see that I have included the following code:

```javascript
for (let c = 0; c < data.length; c++) {
    const date = data[c]['date']
    const dv = data[c]["daily_vaccinations"]
    const dvpm = data[c]["daily_vaccinations_per_million"]

    document.getElementById('v_data').innerHTML += `
        <tr>
            <td>`+ date + `</td>
            <td>`+ dv + `</td>
            <td>`+ dvpm + `</td>
        </tr>
    `
}
```

This code overhere basically dynamically adds the COVID Data recieved through the API, in a tabular format with the *tr* amd *td*. However, if you search a country from the main website, you will see that the data doesn't come in a Tabular Format. 

![table-error](https://user-images.githubusercontent.com/78216399/138656109-2545f194-3619-421e-ba2a-f388aab200f7.png)
