<!SLIDE center #plugins>

# Plugins

<!SLIDE #plugins>

    @@@ ruby
    Scamp.new do |bot|
      bot.plugin MyPlugin

      bot.connect!
    end

<!SLIDE center #plugins>

# Super Simple API

<!SLIDE #plugins>

    @@@ ruby
    class MyPlugin < Scamp::Plugin
      match /^ping$/, :say_pong

      def say_pong room, msg
        room.say "pong"
      end
    end

<!SLIDE center #plugins>

## Speak to me after if you want to write a plugin!
