# Use below code and replace parameter

```ruby
uri = URI::HTTPS.build(:host => "www.whatsappapi.in", :port => 80) 
uri.path = URI.escape("/api") 
client = Net::HTTP.new("www.whatsappapi.in", "80") 
req = Net::HTTP::Post.new(uri.request_uri, {}) 
req.set_form_data({"token" => "Your-Token", "action" => "text", "from" => "919876*****", "country" => "91", "to" => "9876*****", "text" => "Sample Text Message", "uid" => "12324565"}) 
res = client.request(req)
```
