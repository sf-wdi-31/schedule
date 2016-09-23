# Using Ruby Koans

1. Go to the [Ruby Koans website](http://rubykoans.com/) and click the link to download the koans. Extract the zip file into a directory of your choice. From terminal, `cd` into the koans directory and run `ls`. Wow, that's a lot of files!

1. Each file is a self-contained exercise that will teach you a bit about Ruby, using test driven development with a zen flair. Essentially, you will be given code that has something wrong with it, as well as instructions about what needs to be fixed. You'll achieve enlightenment by making the necessary changes for the tests to pass.

  For example, you could use this command to run `about_hashes.rb` in the Terminal:
  ```bash
  :> ruby about_hashes.rb
  ```
  
  Here's what the output might look like:
  ```ruby
  AboutHashes#test_creating_hashes has damaged your karma.
  
  The Master says:
    You have not yet reached enlightenment.
  
  The answers you seek...
    Expected "FILL ME IN" to equal Hash
  
  Please meditate on the following code:
    about_hashes.rb:6:in `test_creating_hashes'
  
  mountains are merely mountains
  your path thus far [X_________________________________________________] 0/12
  ```

1. Each koan file has blanks you should fill or lines you should change to "reach enlightenment."  Read the comments in a koan file one by one to see what each part should do. If you're unsure what one of the tests is asking for, try a few things, ask in Slack, and skip it if you need to (don't get stuck!).

1. The koan files have some structures we haven't gone over yet:
  
  * Methods are defined by the blocks that start with `def` and end with `end` -- these reserved words are like the curly brackets of Ruby methods.  Note that when a method is called, it doesn't need parentheses.    
  * Assert statements say something should be true. For instance `assert_equal hash.size, 2` means that the hash should have 2 things in it. This is also an example of a method call without parentheses. 
  * The `class`  in each file is a way of organizing the code and grouping the methods together.

1. Here's an example of a partially complete koan (from `about_hashes.rb`):

```ruby
require File.expand_path(File.dirname(__FILE__) + '/neo')

class AboutHashes < Neo::Koan
  def test_creating_hashes
    empty_hash = Hash.new
    assert_equal Hash, empty_hash.class
    assert_equal({}, empty_hash)
    assert_equal 0, empty_hash.size
  end

  def test_hash_literals
    hash = { :one => "uno", :two => "dos" }
    assert_equal 2, hash.size
  end

  def test_accessing_hashes
    hash = { :one => "uno", :two => "dos" }
    assert_equal "uno", hash[:one]
    assert_equal "dos", hash[:two]
    assert_equal nil, hash[:doesnt_exist]
  end
end
```

