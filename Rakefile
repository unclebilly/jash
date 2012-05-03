require 'rake/clean'

HERE = File.dirname(__FILE__)
CLEAN.include(File.join(HERE, "dist/*"))

desc "Minimize jash and copy files to dist folder"
task :build => [:clean, :copy] do 
	cp File.join(HERE, "LICENSE"), File.join(HERE, "dist/Jash.js")
	exec "#{File.join(HERE,'lib/jsmin.rb')} < #{File.join(HERE, "src/Jash_source.js")} > #{File.join(HERE, "dist/Jash.js")}"
end

task :copy do
	cp Dir[File.join(HERE, "src/*")], File.join(HERE, "dist/")
end



# jsmin = File.join(File.dirname(__FILE__), "lib/jsmin.rb")
# infile = File.join(File.dirname(__FILE__), "src/Jash_source.js")
# cssin = File.join(File.dirname(__FILE__), "src/Jash.css")
# outfile = File.join(File.dirname(__FILE__), "dist/Jash.js")
# license = File.join(File.dirname(__FILE__), "LICENSE")

# `cat #{license} > #{outfile}`
# `#{jsmin} < #{infile} >> #{outfile}`
