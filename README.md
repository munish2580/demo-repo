require 'thor'

class MyTask < Thor
  desc "hello NAME", "say hello to NAME"
  def hello(name)
    puts "Hello #{name}, I am a Thor task!"
  end
end

MyTask.start(ARGV)
