# Week 6 Training

The evening trainings and readings below will help you solidify work so far and/or prepare you for the next day's materials.

### Monday

1. Practice with directives!  Choose another UI Bootstrap directive, and add it to your Cards Against Assembly app. Be sure to read the known issues for the directive you choose. Try using the directive's settings to customize it for your page.  

1. Get ready for promises! Spend about 40-60 minutes investigating promises with the resources below:
  * Read the first half of  this [cartoon explanation of promises](http://andyshora.com/promises-angularjs-explained-as-cartoon.html), by Andy Shora. (Stop before "What does this look like in code?")
  * Read the "Description" section of MDN's [JavaScript Promise documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise#Description). What an awesome diagram!
  * Watch this 10-minute video on [Angular's `$q` service](https://www.youtube.com/watch?v=W2PBVEgMijo).
  * With any remaining time, briefly look over Angular's [`$q` documentation](https://docs.angularjs.org/api/ng/service/$q) - we'll be using the Deferred API and Promise API (like in the video) instead of `$q` constructor syntax.

1. Based on your research, either answer each of the following questions or write a new, more specific question about the topic:
  * What is a promise?
  * What does it mean for a promise to be pending, fulfilled, resolved, and rejected?
  * How does promise "chaining" work?
  * Draw the lifecycle of a promise.  




### Tuesday

1. Spend about an hour continuing work on this morning's [weather directive challenge](https://github.com/sf-wdi-31/making-a-custom-directive). During your work time - whether or not you have successfully completed building the directive - spend some of your time reading through [this solution](https://github.com/sf-wdi-31/weather-directive). Use that example to help you to complete your version.
1. Similarly, spend an hour on the [book app service refactor](https://github.com/sf-wdi-31/angular-services-training) that you began this afternoon. Make sure to review [the solution branch](https://github.com/sf-wdi-31/angular-services-training/tree/solution-31). Additionally, read [the code from the ngResource solution branch](https://github.com/sf-wdi-31/angular-services-training/tree/ngResource-solution). This is a different approach that Angular provides that drastically reduces the complexity of the code you need to write, but inherently hides a lot of the specifics behind the Angular scenes. A `$resource` is automatically CRUD-able!

### Wednesday

Angular build!

### Thursday

Angular build!

### Weekend

1. Work through [Try Ruby](http://tryruby.org/levels/1/challenges/0), an interactive introduction to Ruby. Note: despite what the site says, this will take longer than 15 minutes! Plan to spend an hour or two on this. The whole tutorial is very useful, but at least do levels 1-4.
 
2. Take about fifteen minutes (total) skimming through the following 3 free books on Ruby. Spend a little time really reading the table of contents (if there is one) and seeing what piques your interest. 

 - http://poignant.guide/book/chapter-1.html
 - http://humblelittlerubybook.com/book/html/index.html
 - http://ruby-doc.com/docs/ProgrammingRuby/
 
 - Another great but non-free reading is Practical Object Oriented Design (POODR) by Sandi Metz, chapters 1-3.

3. Choose at least one of these books to read more of, and spend at least an hour with it this weekend. (But also get some rest, it's been a long week!) 

     **reading tips for technical books:**
  - If you are getting bored, skip ahead to something you are more curious about. You can always come back later.
  - Read the about the author, so you know why you should care what they think. After that, skip to chapter 1, or alternatively skip to a chapter you are especially excited about. Don't bother with the introduction, etc. 

5. Complete the following [Ruby Koans website](http://rubykoans.com/):

- About Asserts - `about_asserts.rb`. This will help you understand how the tests are working, but it's a new concept. Remember, don't get stuck.
- About True and False - `about_true_and_false.rb`
- About Nil - `about_nil.rb`
- About Strings - `about_strings.rb`


<details><summary>Click for more information about Ruby Koans</summary>

Go to the [Ruby Koans website](http://rubykoans.com/) and click the link to download the koans. Extract the zip file into a directory of your choice. From terminal, `cd` into the koans directory and run `ls`. Wow, that's a lot of files!

Each file is a self-contained exercise that will teach you a bit about Ruby, using test driven development with a zen flair. Essentially, you will be given code that has something wrong with it, as well as instructions about what needs to be fixed. You'll achieve enlightenment by making the necessary changes for the tests to pass.

For example, you could use this command to run `about_hashes.rb` in the Terminal:
```bash
:> ruby about_hashes.rb
```
<details><summary>click to see output</summary>
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
</details>

Each koan file has some blanks you should fill or lines you should change to "reach enlightenment."  Read the comments in a koan file one by one to see what each part should do. If you're unsure what one of the tests is asking for, try a few things, ask in Slack, and skip it if you need to (don't get stuck!).

The koan files have some structure we haven't gone over yet:

* Methods are defined by the blocks that start with `def` and end with `end` -- these reserved words are like the curly brackets of Ruby methods.  Note that when a method is called, it doesn't need parentheses.    
* Assert statements say something should be true. For instance `assert_equal hash.size, 2` means that the hash should have 2 things in it. This is also an example of a method call without parentheses. 
* The `class`  in each file is a way of organizing the code and grouping the methods together.

<details><summary>Click for an example of completing parts of a koan (from `about_hashes.rb`):</summary>

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

</details></details>
