# HTI (Hidden Trackable Information) in board games

[Current list](https://agt-the-walker.github.io/board/). I am looking for the
following strings:

* "confidential"
* "down" (this includes "facedown", etc.)
* "hid" (this includes "hidden", etc.)
* "private"
* "public"
* "secret"

# Utilities

## Purpose

### games\_in\_geeklists

Print all games in the public geeklists of the given
[BoardGameGeek](https://boardgamegeek.com/) username in XML format.

### json\_stats

Print some statistics (such as a playing time and rank) from a list of games in
XML format (possibly generated by `games_in_geeklists`)

## Requirements

* [Ruby](http://www.ruby-lang.org/en/) 2.0+
* [Nokogiri](https://rubygems.org/gems/nokogiri) gem

## Usage

    $ ./games_in_geeklists 'Agt the Walker' | ./json_stats >board.json

This generated [board.json](https://agt-the-walker.github.io/board.json), and
can be used to display something like
[board.html](https://agt-the-walker.github.io/board.html).
