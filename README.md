# utl-array-option-i-did-not-know-existed-and-does-not-appear-to-be-documented
Array option I did not know existed and does not appear to be documented?
    Array option I did not know existed and does not appear to be documented?
    First saw Paul Dorfman using this with HASH

    Thanks Paul, I leaned something new.

    github
    https://tinyurl.com/y4hek56v
    https://github.com/rogerjdeangelis/utl-array-option-i-did-not-know-existed-and-does-not-appear-to-be-documented

    * nVar replaces the automatic _i_ iterator in do over;
    data strange;
      set sashelp.class(obs=1);
      array nums  (nVar) age weight height;
      do over nums;
        put nVar=;
      end;
    run;quit;

    NVAR=1
    NVAR=2
    NVAR=3

    * _i_ default;
    data strange;
      set sashelp.class(obs=1);
      array nums age weight height;
      do over nums;
        put _i_=;
      end;
    run;quit;

    _I_=1
    _I_=2
    _I_=3
