# Challenge Name
An Epic Filesystem Quest
## My solve
**Flag:** `pwn.college{YkIIdvz56xGLIiJDTMBH1VbPH4N.QX5IDO0wSO0EzNzEzW}`

```bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
BRIEF  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat BRIEF
Yahaha, you found me!
The next clue is in: /usr/include/fflas-ffpack/fflas

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/include/fflas-ffpack/fflas
hacker@commands~an-epic-filesystem-quest:/usr/include/fflas-ffpack/fflas$ ls
SECRET             fflas_fdot.inl      fflas_freduce_mp.inl  fflas_ftrsm.inl      fflas_pfgemm.inl
fflas.h            fflas_fgemm         fflas_freivalds.inl   fflas_ftrsm_mp.inl   fflas_pftrsm.inl
fflas_bounds.inl   fflas_fgemm.inl     fflas_fscal.h         fflas_ftrsm_src.inl  fflas_simd
fflas_enum.h       fflas_fgemv.inl     fflas_fscal.inl       fflas_ftrsv.inl      fflas_simd.h
fflas_fadd.h       fflas_fgemv_mp.inl  fflas_fscal_mp.inl    fflas_helpers.inl    fflas_sparse
fflas_fadd.inl     fflas_fger.inl      fflas_fsyr2k.inl      fflas_igemm          fflas_sparse.h
fflas_fassign.h    fflas_fger_mp.inl   fflas_fsyrk.inl       fflas_level1.inl     fflas_sparse.inl
fflas_fassign.inl  fflas_freduce.h     fflas_ftrmm.inl       fflas_level2.inl
fflas_faxpy.inl    fflas_freduce.inl   fflas_ftrmm_src.inl   fflas_level3.inl
hacker@commands~an-epic-filesystem-quest:/usr/include/fflas-ffpack/fflas$ cat SECRET
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/wget
hacker@commands~an-epic-filesystem-quest:/usr/include/fflas-ffpack/fflas$ cd /opt/busybox/busybox-1.33.2/include/config/feature/wget
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/wget$ ld
/nix/store/mkvc0lnnpmi604rqsjdlv1pmhr638nbd-binutils-2.44/bin/ld: no input files
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/wget$ ls
HINT  authentication.h  https.h  long  openssl.h  statusbar.h  timeout.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/wget$ cat HINT
Tubular find!
The next clue is in: /usr/share/maxima-sage/5.42.2/share/odepack/src
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/wget$ cd /usr/share/maxima-sage/5.42.2/share/odepack/src
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/odepack/src$ ls
CUE           dcfode.lisp  dhels.lisp    dlsodes.lisp  dpjibt.lisp   dscal.lisp    dsrcma.lisp   dusol.lisp   nnfc.lisp
adjlr.lisp    dcopy.lisp   dheqr.lisp    dlsodi.lisp   dpkset.lisp   dsetpk.lisp   dsrcms.lisp   dvnorm.lisp  nnsc.lisp
cdrv.lisp     ddecbt.lisp  dhesl.lisp    dlsodis.lisp  dprep.lisp    dslsbt.lisp   dsrcom.lisp   idamax.lisp  nntc.lisp
cntnzu.lisp   ddot.lisp    dintdy.lisp   dlsodkr.lisp  dprepi.lisp   dsolbt.lisp   dsrcpk.lisp   iumach.lisp  nroc.lisp
daigbt.lisp   dewset.lisp  diprep.lisp   dlsodpk.lisp  dprepj.lisp   dsolpk.lisp   dstoda.lisp   ixsav.lisp   nsfc.lisp
dainvg.lisp   dfnorm.lisp  diprepi.lisp  dlsoibt.lisp  dprepji.lisp  dsolss.lisp   dstode.lisp   jgroup.lisp  odrv.lisp
dainvgs.lisp  dgbfa.lisp   dlhin.lisp    dmnorm.lisp   dprja.lisp    dsolsy.lisp   dstodi.lisp   md.lisp      package.lisp
datp.lisp     dgbsl.lisp   dls001.cmn    dnrm2.lisp    dprjis.lisp   dspigmr.lisp  dstodpk.lisp  mdi.lisp     sro.lisp
datv.lisp     dgefa.lisp   dlsoda.lisp   dorthog.lisp  dprjs.lisp    dspiom.lisp   dstoka.lisp   mdm.lisp     xerrwd.lisp
daxpy.lisp    dgesl.lisp   dlsodar.lisp  dpcg.lisp     drchek.lisp   dsrcar.lisp   dumach.lisp   mdp.lisp     xsetf.lisp
dbnorm.lisp   dhefa.lisp   dlsode.lisp   dpcgs.lisp    droots.lisp   dsrckr.lisp   dumsum.lisp   mdu.lisp     xsetun.lisp
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/odepack/src$ cat CUE
Great sleuthing!
The next clue is in: /usr/lib/ruby/2.7.0/bundler

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/maxima-sage/5.42.2/share/odepack/src$ cd /usr/lib/ruby/2.7.0/bundler
hacker@commands~an-epic-filesystem-quest:/usr/lib/ruby/2.7.0/bundler$ ls -a
.                          feature_flag.rb          plugin                     source_list.rb
..                         fetcher                  plugin.rb                  spec_set.rb
.INSIGHT                   fetcher.rb               process_lock.rb            stub_specification.rb
build_metadata.rb          friendly_errors.rb       psyched_yaml.rb            templates
capistrano.rb              gem_helper.rb            remote_specification.rb    ui
cli                        gem_helpers.rb           resolver                   ui.rb
cli.rb                     gem_remote_fetcher.rb    resolver.rb                uri_credentials_filter.rb
compact_index_client       gem_tasks.rb             retry.rb                   vendor
compact_index_client.rb    gem_version_promoter.rb  ruby_dsl.rb                vendored_fileutils.rb
constants.rb               gemdeps.rb               ruby_version.rb            vendored_molinillo.rb
current_ruby.rb            graph.rb                 rubygems_ext.rb            vendored_persistent.rb
definition.rb              index.rb                 rubygems_gem_installer.rb  vendored_thor.rb
dep_proxy.rb               injector.rb              rubygems_integration.rb    vendored_uri.rb
dependency.rb              inline.rb                runtime.rb                 version.rb
deployment.rb              installer                settings                   version_ranges.rb
deprecate.rb               installer.rb             settings.rb                vlad.rb
dsl.rb                     lazy_specification.rb    setup.rb                   worker.rb
endpoint_specification.rb  lockfile_generator.rb    shared_helpers.rb          yaml_serializer.rb
env.rb                     lockfile_parser.rb       similarity_detector.rb
environment_preserver.rb   match_platform.rb        source
errors.rb                  mirror.rb                source.rb
hacker@commands~an-epic-filesystem-quest:/usr/lib/ruby/2.7.0/bundler$ cat ^C
hacker@commands~an-epic-filesystem-quest:/usr/lib/ruby/2.7.0/bundler$ cat .INSIGHT
Lucky listing!
The next clue is in: /usr/lib/x86_64-linux-gnu/gstreamer-1.0
hacker@commands~an-epic-filesystem-quest:/usr/lib/ruby/2.7.0/bundler$ cd /usr/lib/x86_64-linux-gnu/gstreamer-1.0
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ ls
EVIDENCE  libgstcoreelements.so  libgstcoretracers.so
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ cat EVIDENCE
Great sleuthing!
The next clue is in: /usr/share/icons/hicolor/64x64/status

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ ls /usr/share/icons/hicolor/64x64/status
TRACE-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ cat /usr/share/icons/hicolor/64x64/status/TRACE-TRAPPED
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/include/config/zlib

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ ls /opt/linux/linux-5.4/include/config/zlib
SPOILER-TRAPPED  deflate.h  inflate.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ cat /opt/linux/linux-5.4/include/config/zlib/SPOILER-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Neo-Euler/Size3/Regular
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/gstreamer-1.0$ cd /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Neo-Euler/Size3/Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Neo-Euler/Size3/Regular$ ls
Main.js  TEASER
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Neo-Euler/Size3/Regular$ cat TEASER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{YkIIdvz56xGLIiJDTMBH1VbPH4N.QX5IDO0wSO0EzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
implemented previous knowledge of cd,cat,ls 
and reading a directory without using cd by first finding files in the specified diectory by ls /adress and then cat/adress/filename 

## References 
none
