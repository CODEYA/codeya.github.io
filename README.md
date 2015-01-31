codeya.github.io
================

## 環境構築

### 前提条件

本ドキュメントは以下の環境を前提とする。

```bash
% sw_vers
ProductName:	Mac OS X
ProductVersion:	10.10.1
BuildVersion:	14B25
```

```bash
% ruby --version
ruby 2.2.0p0 (2014-12-25 revision 49005) [x86_64-darwin14]
```

### Github pages 用環境の構築

以下では Github pages にて採用されている Jekyll の動作環境を構築する。
詳細は以下を参照。

* [GitHub Help - Using Jekyll with Pages](https://help.github.com/articles/using-jekyll-with-pages/)

### Bundler のインストール

```bash
% gem install bundler
Successfully installed bundler-1.7.12
Parsing documentation for bundler-1.7.12
Installing ri documentation for bundler-1.7.12
Done installing documentation for bundler after 2 seconds
1 gem installed
```

### Jekyll のインストール

```bash
% cat Gemfile
source 'https://rubygems.org'
gem 'github-pages'
% bundle install
Fetching gem metadata from https://rubygems.org/..........
Resolving dependencies...
Installing RedCloth 4.2.9
Installing i18n 0.7.0
Installing json 1.8.2
Installing minitest 5.5.1
Installing thread_safe 0.3.4
Installing tzinfo 1.2.2
Installing activesupport 4.2.0
Installing blankslate 2.1.2.4
Installing hitimes 1.2.2
Installing timers 4.0.1
Installing celluloid 0.16.0
Installing fast-stemmer 1.0.2
Installing classifier-reborn 2.0.3
Installing coffee-script-source 1.8.0
Installing execjs 2.2.2
Installing coffee-script 2.3.0
Installing colorator 0.1
Installing ffi 1.9.6
Installing gemoji 2.1.0
Installing net-dns 0.8.0
Installing public_suffix 1.4.6
Installing github-pages-health-check 0.2.1
Installing jekyll-coffeescript 1.0.1
Installing jekyll-gist 1.1.0
Installing jekyll-paginate 1.1.0
Installing sass 3.4.9
Installing jekyll-sass-converter 1.2.0
Installing rb-fsevent 0.9.4
Installing rb-inotify 0.9.5
Installing listen 2.8.5
Installing jekyll-watch 1.2.0
Installing kramdown 1.3.1
Installing liquid 2.6.1
Installing mercenary 0.3.5
Installing posix-spawn 0.3.9
Installing yajl-ruby 1.1.0
Installing pygments.rb 0.6.0
Installing redcarpet 3.1.2
Installing safe_yaml 1.0.4
Installing parslet 1.5.0
Installing toml 0.1.2
Installing jekyll 2.4.0
Installing mini_portile 0.6.2
Installing nokogiri 1.6.5
Installing html-pipeline 1.9.0
Installing jekyll-mentions 0.2.1
Installing jekyll-redirect-from 0.6.2
Installing jekyll-sitemap 0.6.3
Installing jemoji 0.4.0
Installing maruku 0.7.0
Installing rdiscount 2.1.7
Installing terminal-table 1.4.5
Installing github-pages 31
Using bundler 1.7.12
Your bundle is complete!
Use `bundle show [gemname]` to see where a bundled gem is installed.
Post-install message from html-pipeline:
-------------------------------------------------
Thank you for installing html-pipeline!
You must bundle Filter gem dependencies.
See html-pipeline README.md for more details.
https://github.com/jch/html-pipeline#dependencies
-------------------------------------------------
```

## Jekyll 設定

Jekyll の設定については以下を参照。

* [Jekyll - Configuration](http://jekyllrb.com/docs/configuration/)

## Jekyll ローカル実行

Jekyll によるローカルサーバー実行は以下の方法で行う。

```bash
% jekyll serve --watch
/Users/me/.gem/gems/gems/liquid-2.6.1/lib/liquid/htmltags.rb:43: warning: duplicated key at line 46 ignored: "index0"
Configuration file: /Users/me/Project/codeya/codeya.github.io/_config.yml
            Source: /Users/me/Project/codeya/codeya.github.io
       Destination: /Users/me/Project/codeya/codeya.github.io/_site
      Generating...
                    done.
 Auto-regeneration: enabled for '/Users/me/Project/codeya/codeya.github.io'
Configuration file: /Users/me/Project/codeya/codeya.github.io/_config.yml
    Server address: http://0.0.0.0:4000/
  Server running... press ctrl-c to stop.
```
