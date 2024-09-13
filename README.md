# WHOIS Lookup API 🔍🌐
The WHOIS Lookup API provides quick and easy access to domain registration information. This powerful tool allows developers to retrieve essential details about multiple domains simultaneously.

# Endpoint: Multi-Domains Age 📅🔢
This endpoint allows you to fetch the age and creation date for multiple domains in a single request.

# Request 🔍
POST https://whois-lookup-api.p.rapidapi.com/multi-domains-age


## Headers
- Content-Type: application/json
- x-rapidapi-host: whois-lookup-api.p.rapidapi.com
- x-rapidapi-key: YOUR_RAPIDAPI_KEY

# Response 📊
The API returns a JSON object containing subcategories and their details:

# Body
An array of domain names (strings) to look up. The API can handle both bare domains and full URLs.

## Parameters

|       Property         |Type                          |Description|
|----------------|-------------------------------|-----------------------------|
|    domain      |      string                   |The domain name   
| age  |      integer                   |Age of the domain in days  
| creation    |      string                  |Creation date of the domain (YYYY-MM-DD)

# Example 💡

### Request

```bash
curl --request POST \
  --url https://whois-lookup-api.p.rapidapi.com/multi-domains-age \
  --header 'Content-Type: application/json' \
  --header 'x-rapidapi-host: whois-lookup-api.p.rapidapi.com' \
  --header 'x-rapidapi-key: fd3f1114b1msh3d69719929fe501p1f1b72jsn2432d43bd3d1' \
  --data '["google.com","https://bing.com","https://web.whatsapp.com/","claude.ai","github.com","mit.edu","google.us","amazon.in","https://dotnettutorials.net/","https://donate.wikimedia.org/"]'
```

 # Response

{
    "domain": "bing.com",
    "age": 10452,
    "creation": "1996-01-29"
  }
  

### This endpoint provides a quick way to assess the age and creation date of multiple domains at once. Use it for domain research, competitor analysis, or to verify the legitimacy of websites! 🕵️‍♂️🌍


# [Check WHOIS Lookup API](https://rapidapi.com/opendatapoint-opendatapoint-default/api/whois-lookup-api/playground)
