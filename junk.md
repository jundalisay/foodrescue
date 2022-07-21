      {{ if isset .Params "symboliclink" }}
        <a href="{{ .Params.symboliclink }}"{{ if .Params.external }} target="_blank"{{end}}>{{ .Title }}</a>
      {{else}}

      {{ end }}


    <p>{{ .Description | default .Content | plainify | htmlUnescape | truncate 180 "…" }}</p>

{{ if ($.Get "signup" | default true) }}<strong>Sign up to be notified of new rescues!</strong>{{ end }}

{{< home-subscribe >}}

[build]
  command = "hugo"
  publish = "public"

[build.environment]
  HUGO_VERSION = "YOUR_HUGO_VERSION"
