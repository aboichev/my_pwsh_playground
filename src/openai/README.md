curl https://api.openai.com/v1/models \
  -H 'Authorization: Bearer YOUR_API_KEY' \
  -H 'OpenAI-Organization: org-LCY8zwrDmXxRdDBILZnFuXZG



$RequestParms = @{
    Uri = 'https://api.openai.com/v1/models'
    Headers = @{
        "Authorization" = "Bearer " + $env:OPENAI_KEY
    }
}

$response = Invoke-WebRequest @RequestParms