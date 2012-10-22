# A sample Guardfile
# More info at https://github.com/guard/guard#readme

LATEXMK_OPTS = '-pdf -pdflatex=lualatex -recorder'

# Add files and commands to this file, like the example:
#   watch(%r{file/path}) { `command(s)` }
#
guard 'shell' do
  watch(/([^.].*)\.tex$/) do |m|
    `latexmk #{LATEXMK_OPTS} training-short-talk-handouts`
  end
end
