<!SLIDE center #adapters>

# Adapters

<!SLIDE #adapters>

    @@@ ruby
    Scamp.new do |bot|
      bot.adapter :campfire, 
                  Scamp::Campfire::Adapter, 
                  subdomain: 'nwrug',
                  api_key: 'as89...',
                  rooms: [12345]

      bot.connect!
    end

<!SLIDE center #adapters>

# Run Multiple adapters
## Even of the same type!

<!SLIDE center #adapters>

# Super Simple API

<!SLIDE #adapters>

    @@@ ruby
    class TestAdapter < Scamp::Adapter
      def connect!
        push [nil, 
          Scamp::Message.new(body: "Hello")]
      end
    end

<!SLIDE center #adapters>

## Currently have adapters for IRC & Campfire

<!SLIDE center #adapters>

## Speak to me after if you want to write another!
