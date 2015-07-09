task :default => ['build', 'clean', 'open']

name = 'slide'

task :build do
  puts `platex -kanji=UTF8 #{name}.tex`
  puts `platex -kanji=UTF8 #{name}.tex`
  puts `dvipdfmx #{name}.dvi`
end

task :clean do
  `rm *.aux *.dvi *.log *.nav *.out *.snm *.toc`
end

task :open do
  `open #{name}.pdf`
end
