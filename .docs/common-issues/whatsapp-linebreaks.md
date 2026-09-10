# Preserve line breaks in WhatsApp drafts

When building a WhatsApp URL, `encodeURIComponent` should receive a string joined with the JavaScript newline escape `\n`. A doubled escape sends the two visible characters `\\n` to the recipient instead of a line break. Keep long free-text answers on their own line so an admin can scan the request quickly.
