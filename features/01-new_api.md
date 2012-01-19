<!SLIDE center #api>

# New API

<!SLIDE #api>

    @@@ ruby
    Scamp.new do |bot|
      bot.match /^ping$/ do |room, msg|
        room.say "pong"
      end

      bot.connect!
    end

<!SLIDE center #api>

## No more instance eval hacks

<!SLIDE center #api>

## Less Pretty :(

<!SLIDE center #api>

## Way More Flexible!
