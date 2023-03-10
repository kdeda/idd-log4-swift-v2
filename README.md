# Log4swift

Simple logging API for Swift platforms.
Using https://github.com/apple/swift-log.git
Inspired by https://github.com/crspybits/swift-log-file.git

## Log Spamming
To block spamming messages, ie: CVDisplayLinkStart and stuff

Run Console.app
Start streaming
Filter for your noise ie: CVDisplayLinkStart
Locate the Subsystem ie: com.apple.corevideo

Now tell log config to block these.
sudo log config --mode "level:off" --subsystem com.apple.corevideo

