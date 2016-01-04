%w(3.2 4.0 4.1 4.2).each do |version|
  appraise "rails.#{version}.activerecord" do
    gem 'activerecord', "~> #{version}.0"
    gem 'activesupport', "~> #{version}.0"
    gem 'activejob', "~> #{version}.0" if version >= '4.2'
    gem 'resque', require: false
    gem 'sidekiq', require: false
    gem 'sidekiq-unique-jobs', '3.0.14', require: false
  end

  appraise "rails.#{version}.activerecord.kaminari" do
    gem 'activerecord', "~> #{version}.0"
    gem 'activesupport', "~> #{version}.0"
    gem 'activejob', "~> #{version}.0" if version >= '4.2'
    gem 'kaminari', '0.16.3', require: false
  end

  appraise "rails.#{version}.activerecord.will_paginate" do
    gem 'activerecord', "~> #{version}.0"
    gem 'activesupport', "~> #{version}.0"
    gem 'activejob', "~> #{version}.0" if version >= '4.2'
    gem 'will_paginate', require: false
  end
end

%w(4.0 4.1 4.2).each do |version|
  appraise "rails.#{version}.mongoid" do
    gem 'mongoid', '~> 4.0.0'
    gem 'activesupport', "~> #{version}.0"
    gem 'resque', require: false
    gem 'sidekiq', require: false
    gem 'sidekiq-unique-jobs', '3.0.14', require: false
  end

  appraise "rails.#{version}.mongoid.kaminari" do
    gem 'mongoid', '~> 4.0.0'
    gem 'activesupport', "~> #{version}.0"
    gem 'kaminari', '0.16.3', require: false
  end

  appraise "rails.#{version}.mongoid.will_paginate" do
    gem 'mongoid', '~> 4.0.0'
    gem 'activesupport', "~> #{version}.0"
    gem 'will_paginate', require: false
  end
end

appraise "sequel.4.28" do
  gem 'sequel', "~> 4.28.0"
  gem 'activesupport', '~> 4.2.0'
end
