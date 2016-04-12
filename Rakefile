desc 'Sleep for n seconds'
task :sleep, [:n] do |t, args|
  sleep args[:n].to_i
  puts Time.now
end

[3, 5, 7].each do |n|
  desc "Sleep for #{n} seconds"
  task "sleep#{n}" do
    Rake::Task[:sleep].execute n: n
  end
end
