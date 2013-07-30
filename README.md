This is an updated implementation of the PECL PHP SVN module at http://pecl.php.net/package/svn.

You can use this module with Subversion 1.7.

This module adds support for the svn_merge() method. It's signature is as follows.

	svn_merge('source url', 'target url') // merge all missing revisions
	
	svn_merge('source url', 'target url', revision) // merge one revision
	
	svn_merge('source url', 'target url', revision, end_revision) // merge range of revisions

	svn_merge('source url', 'target url', array(revision1, revision2, ...)) // merge array of revisions

	svn_merge(string 'source url', string 'target url', mixed int|array revision=0, int end_revision=0)
  
All existing function signatures are the same as documented at http://php.net/manual/en/book.svn.php.

Some function return semantics have changed when compiling against Subversion 1.7.
