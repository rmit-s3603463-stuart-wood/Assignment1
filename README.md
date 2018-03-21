require "nokogiri"
require "open-uri"

@doc = Nokogiri::XML(File.open("emails.xml"))

@doc.xpath('//send_date').each do



|char_element|

  puts char_element.text

  end
