desc 'Sleep for n seconds'
task :sleep, [:n] do |t, args|
  sleep args[:n]
  puts `date`
end

[3, 5, 7].each do |n|
  desc "Sleep for #{n} seconds"
  task "sleep#{n}".to_sym do
    Rake::Task[:sleep].execute n
  end
end
