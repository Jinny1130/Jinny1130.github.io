source "https://rubygems.org"
# 사용하려는 Jekyll 버전을 관리
# 다른 버전을 사용하고 싶다면 아래 버전을 변경, 파일저장 후 `bundle install`을 실행
# `bundle exec`을 사용하여 Jekyll을 실행. eg:
#
#     bundle exec jekyll serve

gem "jekyll", "~> 4.3.4"
# 이 설정은 새 Jekyll 사이트의 기본 theme. 원하는 테마로 변경 가능.
# gem "minima", "~> 2.5"
# GitHub Pages를 사용하려면 위의 "gem "jekyll"" 줄을 제거
# 아래 줄의 주석 처리를 해제 및 적용, 업그레이드를 위해 `bundle update github-pages`를 실행
# gem "github-pages", group: :jekyll_plugins

# 플러그인
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-paginate", "~> 1.1.0"
end

# Windows와 JRuby에는 zoneinfo 파일이 포함되지 않기 때문에 tzinfo-data gem 및 관련 라이브러리를 번들에 추가
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Windows에서 디렉터리를 감시하는 성능을 높이는 도구
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# JRuby 빌드에서 `http_parser.rb` gem을 `v0.6.x` 버전으로 고정
# 이 gem의 최신 버전에는 Java에 해당하는 부분이 없음
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]