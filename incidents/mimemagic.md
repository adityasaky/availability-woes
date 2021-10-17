# mimemagic

In early 2021, a ruby gem called mimemagic was "yanked" when the developer was informed of a license incompatibility. The gem had a dependency on shared-mime-info, which was licensed under GPL-2. mimemagic itself was licensed MIT, which is incompatible with GPL-2.

After the developer yanked mimemagic, it broke Ruby on Rails, a popular web development framework. While the developer temporarily reinstated a version of the gem to allow packages to proceed, the Rails team eventually switched to a different package.

## Sources

1. Original GitHub issue about license inconsistency: https://github.com/mimemagicrb/mimemagic/issues/97, archived at https://archive.is/W5wGW
2. Yanking breaks Rails: https://github.com/mimemagicrb/mimemagic/issues/98, archived at https://archive.is/d4PWo
3. The Register article about original license inconsistency: https://www.theregister.com/2021/03/25/ruby_rails_code/
4. The Register article about Rails moving to alternative: https://www.theregister.com/2021/03/29/rails_mime_fix/

## Alternative Write Ups

1. ["Dislodging mimemagic And Understanding MIT & GNU GPL." by Emmanuel Hayford](https://emmanuelhayford.com/dislodging-mimemagic-and-understanding-mit-gnu-gpl/)