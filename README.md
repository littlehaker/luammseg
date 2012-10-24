### Install
After cloning, type make.
cp all .o file to lua/ directory.
cd lua/
run make.sh
cp mmseg.so to /usr/local/lib/lua/5.1/

### Usage


	require 'mmseg'

	mmseg.initdict('your_dict_path')
	local ret = mmseg.segment('sentence here')

	print('here is the result:')
	for _, word in ipairs(ret) do
		print(word)
	end
