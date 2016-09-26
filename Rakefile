require 'jekyll'

task :build do
  options = {
    'trace'       => true,
    'verbose'     => true,
    'config' => %w(_config.yml _config_local.yml)
  }
  Jekyll::Commands::Build.process(options)
end

task :serve do
  options = {
    'serving'     => true,
    'watch'       => true,
    'incremental' => true,
    'config'      => %w(_config.yml _config_local.yml)
  }
  Jekyll::Commands::Build.process(options)
  Jekyll::Commands::Serve.process(options)
end