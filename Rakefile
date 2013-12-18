require 'erb'

class SlideshowGenerator
  def self.generate
    slideshow = new
    slideshow.generate
  end

  def template
    File.read('slideshow.html.erb')
  end

  def slide_content
    slide_files.map {|f| File.read(f) }.join("\n---\n")
  end

  def slide_files
    Dir.glob("./slides/**.md").sort
  end

  def generate
    File.write('slideshow.html', ERB.new(template).result(binding))
  end
end

task :generate do
  SlideshowGenerator.generate
end
