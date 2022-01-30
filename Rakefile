task :default do
  sh <<-EOS
curl -o style.json \
https://gsi-cyberjapan.github.io/gsivectortile-mapbox-gl-js/std.json
charites convert style.json style.yml
charites build style.yml docs/style.json
  EOS
end

task :host do
  sh "budo -d docs"
end

